---
title: "XPSSaveAsImage"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Converteert de XPS naar afbeelding"
type: docs
weight: 10
url: /nl/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Converteert de Postscript naar afbeelding.

```js
function AsposeXPSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van het bronlettertype voor conversie. |
| fileName | string | Bestandsnaam. |
| imageFormat | ImageFormat | beeldformaat om naar te converteren. |
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

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
