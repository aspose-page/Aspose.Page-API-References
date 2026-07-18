---
title: "AsposeResizeEPS"
second_title: "Aspose.Page för JavaScript via C++"
description: "Ändra storlek på EPS"
type: docs
weight: 10
url: /sv/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Ändrar storlek på EPS-fil. Den sparar den ursprungliga EPS-filen med en uppdaterad befintlig %%BoundingBox eller en ny skapas.

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

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll i källfilen. |
| fileName | string | Källfilens namn. |
| fileNameResult | string | Resultatfilens namn. |
| width | float | Anger bredden på den nya omgivningsrutan. |
| height | float | Anger höjden på den nya omgivningsrutan. |
| unit | Module.Units | Anger typ av ny storlek. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Se även

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
