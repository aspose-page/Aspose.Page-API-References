---
title: "AsposeResizeEPS"
second_title: "Aspose.Page voor JavaScript via C++"
description: "EPS-grootte wijzigen"
type: docs
weight: 10
url: /nl/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Wijzigt de grootte van een EPS-bestand. Het slaat het oorspronkelijke EPS-bestand op met een bijgewerkte bestaande %%BoundingBox of er wordt een nieuwe aangemaakt.

```js
function AsposeResizeEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    width,
    height,
    units
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van bronbestand. |
| fileName | string | Naam van bronbestand. |
| fileNameResult | string | Naam van resultaatbestand. |
| width | float | Specificeert de breedte van het nieuwe begrenzingsvak. |
| height | float | Specificeert de hoogte van het nieuwe begrenzingsvak. |
| unit | Module.Units | Specificeert het type van de nieuwe grootte. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
