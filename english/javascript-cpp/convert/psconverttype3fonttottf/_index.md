---
title: AsposePSConvertType3FontToTTF
second_title: Aspose.Page for JavaScript via C++
description: Converts PostScript Type 3 fonts to TrueType
type: docs
weight: 10
url: /javascript-cpp/convert/psconverttype3fonttottf/
---
## AsposePSConvertType3FontToTTF function

Converts PostScript Type 3 fonts to TrueType (TTF) and saves the generated font files in the specified directory in the in-memory file system.

```js
function AsposePSConvertType3FontToTTF(
    fileBlob,
    fileName,
    outputDir
)
```

| Parameter | Type | Description |
| --------- | ---- | ----------- |
| fileBlob | ArrayBuffer | Content of the source font file, obtained with FileReader.readAsArrayBuffer. |
| fileName | string | Source font file name. |
| outputDir | string | Directory for the generated TTF files in the in-memory file system. Create it with FS.mkdirTree before conversion. |

### Return Value

JSON object.

| Field | Description |
| ----- | ----------- |
| errorCode | Error code (0 indicates success). |
| errorText | Error message (empty on success). |
| outputDir | Directory containing the generated TTF font files. |

Enumerate the TTF files in `json.outputDir` using `FS.readdir`. Conversion can produce multiple font files. Use a fresh output directory for each conversion to avoid including files from previous calls.

### Examples

Run the following code after the library has initialized. `DownloadFile` is provided by `AsposePageforJS.js` and reads each font from the in-memory file system.

```js
  var fontConversionId = 0;

  // The C++ conversion functions return outputDir; discover the TTF files in that directory.
  var collectTtfFiles = function (directory) {
    const files = [];
    for (const name of FS.readdir(directory)) {
      if (name === '.' || name === '..') continue;
      const path = directory + '/' + name;
      if (FS.isDir(FS.stat(path).mode)) files.push(...collectTtfFiles(path));
      else if (/\.ttf$/i.test(name)) files.push(path);
    }
    return files;
  };

  var convertPsFontToTTF = function (e, convertFont, fontType) {
    const file = e.target.files[0];
    if (!file) return;
    const file_reader = new FileReader();
    file_reader.onerror = () => {
      document.getElementById('output').textContent = 'Unable to read the font file.';
    };
    file_reader.onload = (event) => {
      try {
        // Use a fresh directory so earlier conversions do not appear in the result.
        const outputDir = '/font-conversion/' + fontType + '-' + Date.now() + '-' + (++fontConversionId);
        FS.mkdirTree(outputDir);
        const json = convertFont(event.target.result, file.name, outputDir);
        if (json.errorCode != 0) {
          document.getElementById('output').textContent = json.errorText;
          return;
        }
        const files = collectTtfFiles(json.outputDir);
        document.getElementById('output').textContent = files.length
          ? 'TTF files count: ' + files.length : 'No TTF files were generated.';
        for (const path of files) DownloadFile(path, 'font/ttf');
      }
      catch (error) {
        document.getElementById('output').textContent = error.message;
      }
    };
    file_reader.readAsArrayBuffer(file);
  };



  var fPSConvertType3FontToTTF = function (e) {
    convertPsFontToTTF(e, AsposePSConvertType3FontToTTF, 'type3');
  };
```

**Web Worker example**:

The default library worker handler expects `fileNameResult`. The following example embeds an adapter in a Blob worker to handle `outputDir` and transfer all generated TTF files. The adapter adds `filesCount` and `filesNameResult` to the response JSON; these fields are not returned by `AsposePSConvertType3FontToTTF` itself. Absolute URLs allow the Blob worker to load the library, WASM and settings files.

In the main thread, wait for the `ready` message before allowing file selection. The page must contain elements with IDs `output` and `fileDownload`.

```js
  // Inline worker adapter for font conversions returning outputDir.
  const fontWorker = function (baseUrl) {
    // Blob workers need absolute URLs for the library, WASM and settings files.
    self.Module = {
      locateFile: path => new URL(path, baseUrl).href
    };
    const originalFetch = self.fetch.bind(self);
    self.fetch = (input, options) => originalFetch(
      typeof input === 'string' ? new URL(input, baseUrl).href : input, options);
    // Example-only adapter: the library's default worker expects fileNameResult,
    // whereas font conversion returns outputDir and can generate multiple TTF files.
    // Register before importScripts so font messages bypass the default handler.
    self.addEventListener('message', function (event) {
      const operation = event.data.operation;
      if (operation !== 'AsposePSConvertType1FontToTTF' &&
          operation !== 'AsposePSConvertType3FontToTTF') return;
      event.stopImmediatePropagation();

      let json;
      const params = [];
      const transfer = [];
      try {
        FS.mkdirTree(event.data.params[2]);
        json = self[operation](...event.data.params);
        if (json.errorCode == 0) {
          const files = [];
          const collectTtfFiles = function (directory) {
            for (const name of FS.readdir(directory)) {
              if (name === '.' || name === '..') continue;
              const path = directory + '/' + name;
              if (FS.isDir(FS.stat(path).mode)) collectTtfFiles(path);
              else if (/\.ttf$/i.test(name)) files.push(path);
            }
          };
          collectTtfFiles(json.outputDir);
          json.filesNameResult = files;
          json.filesCount = files.length;
          for (const path of files) {
            const content = FS.readFile(path);
            params.push(content);
            transfer.push(content.buffer);
          }
        }
      }
      catch (error) {
        json = { errorCode: 1, errorText: error.message };
        params.length = 0;
        transfer.length = 0;
      }
      self.postMessage({ operation: operation, json: json, params: params }, transfer);
    });

    // Existing operations keep using the original library worker handler.
    importScripts(new URL('AsposePageforJS.js', baseUrl).href);
  };
  const workerUrl = URL.createObjectURL(new Blob([
    '(' + fontWorker.toString() + ')(' + JSON.stringify(new URL('.', document.baseURI).href) + ');'
  ], { type: 'text/javascript' }));
  const AsposePageWebWorker = new Worker(workerUrl);
  let fontConversionId = 0;
  AsposePageWebWorker.onerror = evt => console.log(`Error from Web Worker: ${evt.message}`);
  AsposePageWebWorker.onmessage = evt => {
    if (evt.data === 'ready') {
      URL.revokeObjectURL(workerUrl);
      document.getElementById('output').textContent = 'library loaded!';
      return;
    }
    const { json, params } = evt.data;
    if (json.errorCode != 0) {
      document.getElementById('output').textContent = json.errorText;
      return;
    }
    document.getElementById('output').textContent = json.filesCount
      ? 'TTF files count: ' + json.filesCount : 'No TTF files were generated.';
    for (let i = 0; i < json.filesCount; i++) {
      DownloadFile(json.filesNameResult[i].split('/').pop(), 'font/ttf', params[i]);
    }
  };

  const fPSConvertType3FontToTTF = e => {
    const file = e.target.files[0];
    if (!file) return;
    const file_reader = new FileReader();
    file_reader.onload = event => {
      const outputDir = '/font-conversion/' + Date.now() + '-' + (++fontConversionId);
      AsposePageWebWorker.postMessage({
        operation: 'AsposePSConvertType3FontToTTF',
        params: [event.target.result, file.name, outputDir]
      }, [event.target.result]);
    };
    file_reader.readAsArrayBuffer(file);
  };

  const DownloadFile = (filename, mime, content) => {
    const link = document.createElement('a');
    link.href = URL.createObjectURL(new Blob([content], { type: mime }));
    link.download = filename;
    link.textContent = filename;
    document.getElementById('fileDownload').appendChild(link);
    document.getElementById('fileDownload').appendChild(document.createElement('br'));
  };
```

### See Also

* function [AsposePSConvertType1FontToTTF](../psconverttype1fonttottf/)
