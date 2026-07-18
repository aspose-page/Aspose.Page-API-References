---
title: "XPSSaveAsImage"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Convierte el XPS a imagen"
type: docs
weight: 10
url: /es/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Convierte el Postscript a imagen.

```js
function AsposeXPSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileBlob | Objeto Blob | Contenido de la fuente de origen para la conversión. |
| fileName | string | Nombre del archivo. |
| imageFormat | ImageFormat | formato de imagen al que convertir. |
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

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
