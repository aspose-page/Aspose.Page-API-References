---
title: "XPSSaveAsPdf"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Convierte el XPS a PDF"
type: docs
weight: 10
url: /es/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

Convierte el XPS a PDF.

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileBlob | Objeto Blob | Contenido de la fuente de origen para la conversión. |
| fileName | string | Nombre del archivo. |
| supressErrors | bool | Especifica si los errores deben suprimirse o no. |

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

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsPdf(xps_file,true);
    console.log("XPSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [XPSSaveAsImage](../xpssaveasimage/)
