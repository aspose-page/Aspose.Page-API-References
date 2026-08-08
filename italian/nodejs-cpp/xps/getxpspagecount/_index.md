---
title: "AsposeGetXpsPageCount"
second_title: "Aspose.Page per JavaScript via C++"
description: "Ottieni il numero di pagine nel file XPS"
type: docs
weight: 10
url: /it/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

Ottieni il numero di pagine nel documento xps.

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| Parametro | Tipo | Descrizione |
| --------- | ---- | ----------- |
| fileBlob | Oggetto Blob | Contenuto del file di origine. |
| fileName | string | Nome del file di origine. |

### Valore di ritorno

oggetto JSON
| Campo | Descrizione |
| ----- | ----------- |
|  | errorCode | errore di codice (0 nessun errore) |
|  | errorText | errore di testo ("" nessun errore) |
|  | pageCount | numero di pagine |

### Esempi

```js
const AsposePage = require('asposepagenodejs');

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    let json = AsposePageModule.AsposePageAbout();
    console.log("AsposePageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : "error:" + json.errorText);

    //AsposeGetXpsPageCount
    json = AsposePageModule.AsposeGetXpsPageCount(xps_file);
    console.log("AsposeGetXpsPageCount => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```


