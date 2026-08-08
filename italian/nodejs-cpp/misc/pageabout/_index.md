---
title: "AsposePageAbout"
second_title: "Aspose.Page per JavaScript via C++"
description: "Ottieni informazioni sul prodotto."
type: docs
url: /it/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Ottieni informazioni sul prodotto.

```js
function AsposePageAbout()
```

### Valore restituito

oggetto JSON
| Campo | Descrizione |
| ----- | ----------- |
| errorCode | errore di codice (0 nessun errore) |
| errorText | errore di testo ("" nessun errore) |
| prodotto | Nome prodotto |
| versione | Versione prodotto |
| islicensed | Il prodotto è con licenza |


```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //PageAbout - Get info about Product
    const json = AsposePageModule.AsposePageAbout();
    console.log("PageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```
