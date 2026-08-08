---
title: "XPSSaveAsPdf"
second_title: "Aspose.Page för JavaScript via C++"
description: "Konverterar XPS till PDF"
type: docs
weight: 10
url: /sv/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

Konverterar XPS till PDF.

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll för källteckensnitt för konvertering. |
| fileName | string | Filnamn. |
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

    const json = AsposePageModule.AsposeXPSSaveAsPdf(xps_file,true);
    console.log("XPSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Se även

* function [XPSSaveAsImage](../xpssaveasimage/)
