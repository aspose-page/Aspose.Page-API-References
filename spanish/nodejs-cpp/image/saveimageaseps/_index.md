---
title: "AsposeSaveImageAsEps"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Redimensionar EPS"
type: docs
weight: 10
url: /es/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

Redimensiona el archivo EPS. Guarda el archivo EPS inicial con el %%BoundingBox existente actualizado o se creará uno nuevo.

```js
function AsposeSaveImageAsEps(
    fileBlob,
    fileName, 
    fileNameResult
)
```

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileBlob | Objeto Blob | Contenido del archivo fuente. |
| fileName | string | Nombre del archivo fuente. |
| fileNameResult | string | Nombre del archivo resultante. |

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

### Ver también

