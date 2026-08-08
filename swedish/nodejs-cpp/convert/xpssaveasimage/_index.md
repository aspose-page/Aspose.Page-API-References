---
title: "XPSSaveAsImage"
second_title: "Aspose.Page för JavaScript via C++"
description: "Konverterar XPS till bild"
type: docs
weight: 10
url: /sv/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Konverterar Postscript till bild.

```js
function AsposeXPSSaveAsImage(
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

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Se även

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
