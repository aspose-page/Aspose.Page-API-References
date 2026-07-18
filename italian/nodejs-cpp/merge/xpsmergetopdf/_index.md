---
title: "AsposeXPSMergeToPdf"
second_title: "Aspose.Page per JavaScript via C++"
description: "Unisci i file XPS in PDF"
type: docs
weight: 10
url: /it/nodejs-cpp/merge/xpsmergetopdf/
---
## AsposeXPSMergeToPdf function

Unisci i file XPS in PDF.

```js
function AsposeXPSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parametro | Tipo | Descrizione |
| --------- | ---- | ----------- |
| fileNames | string | I nomi dei file da unire. |
| fileNameResult | string | Il nome del file PDF risultante. |
| supressErrors | bool | Specifica se gli errori devono essere soppressi o meno. |

### Valore di ritorno

oggetto JSON
| Campo | Descrizione |
| ----- | ----------- |
|  | errorCode | errore di codice (0 nessun errore) |
|  | errorText | errore di testo ("" nessun errore) |
|  | fileNameResult | nome file risultato |

### Esempi

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

### Vedi anche

* function [PSSaveAsImage](../pssaveasimage/)
