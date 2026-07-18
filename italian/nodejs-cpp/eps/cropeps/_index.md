---
title: "AsposeCropEPS"
second_title: "Aspose.Page per JavaScript via C++"
description: "Ritaglia EPS"
type: docs
weight: 10
url: /it/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Ritaglia il file EPS. Salva il file EPS originale con il %%BoundingBox esistente aggiornato oppure ne crea uno nuovo.

```js
function AsposeCropEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    left,
    top,
    right,
    bottom
)
```

| Parametro | Tipo | Descrizione |
| --------- | ---- | ----------- |
| fileBlob | Oggetto Blob | Contenuto del file di origine. |
| fileName | string | Nome del file di origine. |
| fileNameResult | string | Nome del file di risultato. |
| sinistra | float | Specifica il limite sinistro della casella di ritaglio. |
| alto | float | Specifica il limite superiore della casella di ritaglio. |
| destra | float | Specifica il limite destro della casella di ritaglio. |
| inferiore | float | Specifica il limite inferiore della casella di ritaglio. |

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

const eps_file = "./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //CropEPS - working with EPS
    const json = AsposePageModule.AsposeCropEPS(eps_file, "croped.eps", 30, 5, 240, 36);
    console.log("CropEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Vedi anche

* function [AsposeResizeEps](../resizeeps/)
