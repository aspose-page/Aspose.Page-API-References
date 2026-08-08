---
title: "PSSaveAsPdf"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Convierte el Postscript a PDF"
type: docs
weight: 10
url: /es/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Convierte el Postscript a PDF.

```js
function AsposePSSaveAsPdf(
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page para Node.js mediante ejemplos en C++.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Se ha producido un error desconocido: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
