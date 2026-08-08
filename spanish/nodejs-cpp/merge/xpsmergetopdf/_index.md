---
title: "AsposeXPSMergeToPdf"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Combinar los archivos XPS a PDF"
type: docs
weight: 10
url: /es/nodejs-cpp/merge/xpsmergetopdf/
---
## AsposeXPSMergeToPdf function

Combinar los archivos XPS a PDF.

```js
function AsposeXPSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileNames | string | Los nombres de los archivos para combinar. |
| fileNameResult | string | El nombre del archivo PDF resultante. |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToPdf(xps_files,"XPsMergedToPdfResult.pdf");
    console.log("XPSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [PSSaveAsImage](../pssaveasimage/)
