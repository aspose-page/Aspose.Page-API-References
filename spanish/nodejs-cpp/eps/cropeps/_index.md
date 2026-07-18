---
title: "AsposeCropEPS"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Recortar EPS"
type: docs
weight: 10
url: /es/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Recorta el archivo EPS. Guarda el archivo EPS inicial con el %%BoundingBox existente actualizado o se creará uno nuevo.

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

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileBlob | Objeto Blob | Contenido del archivo fuente. |
| fileName | string | Nombre del archivo fuente. |
| fileNameResult | string | Nombre del archivo resultante. |
| izquierda | float | Especifica el límite izquierdo del cuadro de recorte. |
| superior | float | Especifica el límite superior del cuadro de recorte. |
| derecha | float | Especifica el límite derecho del cuadro de recorte. |
| inferior | float | Especifica el límite inferior del cuadro de recorte. |

### Valor de retorno

Objeto JSON
| Campo | Descripción |
| ----- | ----------- |
|  | errorCode | error de código (0 sin error) |
|  | errorText | error de texto ("" sin error) |
|  | fileNameResult | nombre del archivo de resultado |

### Ejemplos

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

### Ver también

* function [AsposeResizeEps](../resizeeps/)
