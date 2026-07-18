---
title: "AsposeSaveImageAsEps"
second_title: "Aspose.Page voor JavaScript via C++"
description: "EPS-grootte wijzigen"
type: docs
weight: 10
url: /nl/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

Wijzigt de grootte van een EPS-bestand. Het slaat het oorspronkelijke EPS-bestand op met een bijgewerkte bestaande %%BoundingBox of er wordt een nieuwe aangemaakt.

```js
function AsposeSaveImageAsEps(
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
|  | fileNameResult | resultaat bestandsnaam |

### Voorbeelden

```js
const AsposePage = require('asposepagenodejs');

const img_file = "./data/PAGENET-361-10.bmp";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //SaveImageAsEps - convert image to EPS
    const json = AsposePageModule.AsposeSaveImageAsEps(img_file, img_file + ".eps");
    console.log("SaveImageAsEps => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

