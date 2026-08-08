---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page voor JavaScript via C++"
description: "XMP-metadata ophalen"
type: docs
weight: 10
url: /nl/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Leest PS/EPS-bestand en extraheert XmpMetdata als deze al bestaat.
Als een EPS-bestand geen XMP-metadata bevat, krijgen we een nieuwe die is gevuld met waarden uit PS-metadata-commentaren (%%Creator, %%CreateDate, %%Title enz.).
EPS-bestand met ingevulde XMP-metadata wordt opgeslagen in fileNameResult.

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van bronbestand. |
| fileName | string | Naam van bronbestand. |
| fileNameResult | string | Naam van resultaatbestand. |


### Retourwaarde

JSON-object
| Veld | Beschrijving |
| ----- | ----------- |
|  | errorCode | codefout (0 geen fout) |
|  | errorText | tekstfout ("" geen fout) |
|  | XMP | array van metadata-waarden |
|  | fileNameResult | resultaat bestandsnaam |

### Voorbeelden

```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeEPSGetXMP(eps_file, img_file + "_out.eps");
    console.log("AsposeEPSGetXMP => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

* function [XPSSaveAsImage](../xpssaveasimage/)
