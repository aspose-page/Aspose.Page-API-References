---
title: "AsposeCropEPS"
second_title: "Aspose.Page för JavaScript via C++"
description: "Beskär EPS"
type: docs
weight: 10
url: /sv/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Beskär EPS-fil. Den sparar den ursprungliga EPS-filen med uppdaterad befintlig %%BoundingBox eller en ny kommer att skapas.

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

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll i källfilen. |
| fileName | string | Källfilens namn. |
| fileNameResult | string | Resultatfilens namn. |
| vänster | float | Anger vänster gräns för beskärningsrutan. |
| övre | float | Anger övre gräns för beskärningsrutan. |
| höger | float | Anger höger gräns för beskärningsrutan. |
| nedre | float | Anger nedre gräns för beskärningsrutan. |

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

### Se även

* function [AsposeResizeEps](../resizeeps/)
