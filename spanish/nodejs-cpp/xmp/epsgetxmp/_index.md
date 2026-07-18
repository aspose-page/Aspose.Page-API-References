---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Obtener metadatos XMP"
type: docs
weight: 10
url: /es/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Lee un archivo PS/EPS y extrae XmpMetdata si ya existe.
Si el archivo EPS no contiene metadatos XMP, obtenemos uno nuevo rellenado con valores de los comentarios de metadatos PS (%%Creator, %%CreateDate, %%Title, etc.).
El archivo EPS con metadatos XMP completados se guardará en fileNameResult.

```js
function AsposeEPSGetXmp(
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
|  | XMP | matriz de valores de metadatos |
|  | fileNameResult | nombre del archivo de resultado |

### Ejemplos

```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeEPSGetXMP(eps_file, img_file + "_out.eps");
    console.log("AsposeEPSGetXMP => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [XPSSaveAsImage](../xpssaveasimage/)
