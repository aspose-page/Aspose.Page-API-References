---
title: "AsposeCropEPS"
second_title: "Aspose.Page voor JavaScript via C++"
description: "EPS bijsnijden"
type: docs
weight: 10
url: /nl/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Bijsnijdt EPS-bestand. Het slaat het oorspronkelijke EPS-bestand op met een bijgewerkte bestaande %%BoundingBox of er wordt een nieuwe aangemaakt.

```js
function AsposeCropEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    left,
    top,
    right,
    bottom
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van bronbestand. |
| fileName | string | Naam van bronbestand. |
| fileNameResult | string | Naam van resultaatbestand. |
| links | float | Specificeert de linkse grens van de bijsnijdingsbox. |
| boven | float | Specificeert de bovenste grens van de bijsnijdingsbox. |
| rechts | float | Specificeert de rechtse grens van de bijsnijdingsbox. |
| onder | float | Specificeert de onderste grens van de bijsnijdingsbox. |

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

const eps_file = "./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //CropEPS - working with EPS
    const json = AsposePageModule.AsposeCropEPS(eps_file, "croped.eps", 30, 5, 240, 36);
    console.log("CropEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

* function [AsposeResizeEps](../resizeeps/)
