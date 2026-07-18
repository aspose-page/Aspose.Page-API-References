---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page per JavaScript via C++"
description: "Ottieni i metadati XMP"
type: docs
weight: 10
url: /it/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Legge il file PS/EPS ed estrae XmpMetdata se esiste già.
Se il file EPS non contiene metadati XMP, ne otteniamo uno nuovo riempito con i valori dei commenti dei metadati PS (%%Creator, %%CreateDate, %%Title ecc).
Il file EPS con i metadati XMP compilati verrà salvato in fileNameResult.

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| Parametro | Tipo | Descrizione |
| --------- | ---- | ----------- |
| fileBlob | Oggetto Blob | Contenuto del file di origine. |
| fileName | string | Nome del file di origine. |
| fileNameResult | string | Nome del file di risultato. |


### Valore di ritorno

oggetto JSON
| Campo | Descrizione |
| ----- | ----------- |
|  | errorCode | errore di codice (0 nessun errore) |
|  | errorText | errore di testo ("" nessun errore) |
|  | XMP | array di valori dei metadati |
|  | fileNameResult | nome file risultato |

### Esempi

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

### Vedi anche

* function [XPSSaveAsImage](../xpssaveasimage/)
