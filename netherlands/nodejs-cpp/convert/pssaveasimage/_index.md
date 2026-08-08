---
title: "PSSaveAsImage"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Converteert de Postscript naar afbeelding"
type: docs
weight: 10
url: /nl/nodejs-cpp/convert/pssaveasimage/
---
## PSSaveAsImage function

Converteert de Postscript naar afbeelding.

```js
function AsposePSSaveAsImage(
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

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSSaveAsImage(ps_file, AsposePageModule.ImageFormat.Png, true);
    console.log("PSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

* function [PSSaveAsPdf](../pssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
