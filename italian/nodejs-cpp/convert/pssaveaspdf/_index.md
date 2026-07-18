---
title: "PSSaveAsPdf"
second_title: "Aspose.Page per JavaScript via C++"
description: "Converte il Postscript in PDF"
type: docs
weight: 10
url: /it/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Converte il Postscript in PDF.

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parametro | Tipo | Descrizione |
| --------- | ---- | ----------- |
| fileBlob | Oggetto Blob | Contenuto del font sorgente per la conversione. |
| fileName | string | Nome file. |
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page per Node.js via esempi C++.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Si è verificato un errore sconosciuto: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
