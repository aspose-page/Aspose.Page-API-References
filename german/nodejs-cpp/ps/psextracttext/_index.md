---
title: "AsposePSExtractText"
second_title: "Aspose.Page für JavaScript über C++"
description: "Text aus PS-Datei extrahieren"
type: docs
weight: 10
url: /de/nodejs-cpp/ps/psextracttext/
---
## AsposePSExtractText function

Text aus PS-Datei extrahieren. Der Text kann nur extrahiert werden, wenn er mit Type 42 (TrueType) oder Type 0 font mit Type 42 fonts in seiner Vector Map geschrieben ist.

```js
function AsposePSExtractText(
    fileBlob,
    fileName, 
    start,
    end
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileBlob | Blob-Objekt | Inhalt der Quelldatei. |
| fileName | string | Name der Quelldatei. |
| Start | int | Gibt die Seite an, ab der Text extrahiert werden soll. Dieser Parameter ist nützlich für mehrseitige Dokumente. |
| Ende | int | Gibt die Seite an, bis zu der Text extrahiert werden soll. Dieser Parameter ist nützlich für mehrseitige Dokumente. |

### Rückgabewert

JSON-Objekt
| Feld | Beschreibung |
| ----- | ----------- |
|  | errorCode | Code-Fehler (0 kein Fehler) |
|  | errorText | Textfehler ("" kein Fehler) |
|  | Text | der extrahierte Text |

### Beispiele

```js
  var fPSExtractText = function (e) {
    const file_reader = new FileReader();
    file_reader.onload = (event) => {
      const json = AsposePSExtractText(event.target.result, e.target.files[0].name);
      if (json.errorCode == 0) {
        document.getElementById('output').textContent = "Text:" + json.text;
      }
      else 
        document.getElementById('output').textContent = json.errorText;
    }
    file_reader.readAsArrayBuffer(e.target.files[0]);
  }
```

**Web Worker example**:
```js

  /*Create Web Worker*/
  const AsposePageWebWorker = new Worker("AsposePageforJS.js");
  AsposePageWebWorker.onerror = evt => console.log(`Error from Web Worker: ${evt.message}`);
  AsposePageWebWorker.onmessage = evt => document.getElementById('output').textContent = 
    (evt.data == 'ready') ? 'library loaded!' :
      (evt.data.json.errorCode == 0) ? 
        ((evt.data.operation == 'AsposePSExtractText') ? `Text: ${evt.data.json.text}` : `` ) : `Error: ${evt.data.json.errorText}`;

  /*Event handler*/
  const fPSExtractText = e => {
    const file_reader = new FileReader();
    file_reader.onload = event => {
      AsposePageWebWorker.postMessage({ "operation": 'AsposePSExtractText', "params": [event.target.result, e.target.files[0].name] }, [event.target.result]);
    };
    file_reader.readAsArrayBuffer(e.target.files[0]);
  };

```

### Siehe auch

* function [AsposePSGetBoundingBox](../psgetboundingbox/)
