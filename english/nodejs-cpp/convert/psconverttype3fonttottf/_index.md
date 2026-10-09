---
title: AsposePSConvertType3FontToTTF
second_title: Aspose.Page for JavaScript via C++
description: Converts PostScript Type 3 fonts to TrueType
type: docs
weight: 10
url: /nodejs-cpp/convert/psconverttype3fonttottf/
---
## AsposePSConvertType3FontToTTF function

Converts PostScript Type 3 fonts to TrueType (TTF) and saves the generated font files in the specified directory in the file system.

```js
function AsposePSConvertType3FontToTTF(
    fileName,
    outputDir
)
```

| Parameter | Type | Description |
| --------- | ---- | ----------- |
| fileName | string | Source font file name. |
| outputDir | string | Directory for the generated TTF files in the in-memory file system. Create it with FS.mkdirTree before conversion. |

### Return Value

JSON object.

| Field | Description |
| ----- | ----------- |
| errorCode | Error code (0 indicates success). |
| errorText | Error message (empty on success). |
| outputDir | Directory containing the generated TTF font files. |

### Examples

Run the following code after the library has initialized. `DownloadFile` is provided by `AsposePageforJS.js` and reads each font from the in-memory file system.

```js
const AsposePage = require('asposepagenodejs');

const ps3_file = "./data/simple_text_alternation_type3.ps";

console.log("Aspose.Page for Node.js via C++ examples.");


AsposePage().then(AsposePageModule => {

    let json = AsposePageModule.AsposePageAbout();
    console.log("AsposePageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : "error:" + json.errorText);

    json = AsposePageModule.AsposePSConvertType3FontToTTF(ps3_file, './data/');
    console.log("AsposePSConvertType3FontToTTF => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### See Also

* function [AsposePSConvertType1FontToTTF](../psconverttype1fonttottf/)
