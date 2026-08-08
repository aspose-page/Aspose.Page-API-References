---
title: "PSSaveAsImage"
second_title: "Aspose.Page för JavaScript via C++"
description: "Konverterar Postscript till bild"
type: docs
weight: 10
url: /sv/nodejs-cpp/convert/pssaveasimage/
---
## PSSaveAsImage function

Konverterar Postscript till bild.

```js
function AsposePSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll för källteckensnitt för konvertering. |
| fileName | string | Filnamn. |
| imageFormat | ImageFormat | bildformat att konvertera till. |
| supressErrors | bool | Anger om fel ska undertryckas eller inte. |

### Returvärde

JSON-objekt
| Fält | Beskrivning |
| ----- | ----------- |
|  | errorCode | kodfel (0 inget fel) |
|  | errorText | textfel ("" inget fel) |
|  | fileNameResult | resultatfilnamn |

### Exempel

```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSSaveAsImage(ps_file, AsposePageModule.ImageFormat.Png, true);
    console.log("PSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Se även

* function [PSSaveAsPdf](../pssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
