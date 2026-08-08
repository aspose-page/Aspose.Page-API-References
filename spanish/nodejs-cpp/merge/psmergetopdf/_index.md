---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Combinar los archivos Postscript a PDF"
type: docs
weight: 10
url: /es/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Combinar los archivos Postscript a PDF.

```js
function AsposePSMergePdf(
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [PSSaveAsImage](../pssaveasimage/)
