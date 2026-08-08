---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Combinar los archivos XPS en un solo XPS"
type: docs
weight: 10
url: /es/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Combinar varios archivos XPS en un solo archivo XPS.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parámetro | Tipo | Descripción |
| --------- | ---- | ----------- |
| fileNames | string | Los nombres de los archivos para combinar. |
| fileNameResult | string | El nombre del archivo XPS resultante. |
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

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Ver también

* function [XPSMergeToPdf](../xpsmergetopdf/)
