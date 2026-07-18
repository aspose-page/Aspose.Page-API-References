---
title: "AsposeResizeEPS"
second_title: "Aspose.Page per JavaScript via C++"
description: "Ridimensiona EPS"
type: docs
weight: 10
url: /it/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Ridimensiona il file EPS. Salva il file EPS originale con il %%BoundingBox esistente aggiornato o ne crea uno nuovo.

```js
function AsposeResizeEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    width,
    height,
    units
)
```

| Parametro | Tipo | Descrizione |
| --------- | ---- | ----------- |
| fileBlob | Oggetto Blob | Contenuto del file di origine. |
| fileName | string | Nome del file di origine. |
| fileNameResult | string | Nome del file di risultato. |
| larghezza | float | Specifica la larghezza del nuovo bounding box. |
| altezza | float | Specifica l'altezza del nuovo bounding box. |
| unità | Module.Units | Specifica il tipo della nuova dimensione. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Vedi anche

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
