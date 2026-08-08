---
title: "XPSSaveAsPdf"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Converteert de XPS naar PDF"
type: docs
weight: 10
url: /nl/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

Converteert de XPS naar PDF.

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van het bronlettertype voor conversie. |
| fileName | string | Bestandsnaam. |
| supressErrors | bool | Specificeert of fouten al dan niet onderdrukt moeten worden. |

### Retourwaarde

JSON-object
| Veld | Beschrijving |
| ----- | ----------- |
|  | errorCode | codefout (0 geen fout) |
|  | errorText | tekstfout ("" geen fout) |
|  | fileNameResult | resultaat bestandsnaam |

### Voorbeelden

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

### Zie ook

* function [XPSSaveAsImage](../xpssaveasimage/)
