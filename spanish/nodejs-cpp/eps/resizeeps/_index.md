---
title: "AsposeResizeEPS"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Redimensionar EPS"
type: docs
weight: 10
url: /es/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Redimensiona el archivo EPS. Guarda el archivo EPS inicial con el %%BoundingBox existente actualizado o se creará uno nuevo.

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

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileBlob | Objeto Blob | Contenido del archivo fuente. |
| fileName | string | Nombre del archivo fuente. |
| fileNameResult | string | Nombre del archivo resultante. |
| width | float | Especifica el ancho del nuevo cuadro delimitador. |
| height | float | Especifica la altura del nuevo cuadro delimitador. |
| unit | Module.Units | Especifica el tipo del nuevo tamaño. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
