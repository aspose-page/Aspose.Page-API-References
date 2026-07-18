---
title: "AsposePageAbout"
second_title: "Aspose.Page für JavaScript über C++"
description: "Informationen zum Produkt abrufen."
type: docs
url: /de/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Informationen zum Produkt abrufen.

```js
function AsposePageAbout()
```

### Rückgabewert

JSON-Objekt
| Feld | Beschreibung |
| ----- | ----------- |
| errorCode | Code-Fehler (0 kein Fehler) |
| errorText | Textfehler ("" kein Fehler) |
| Produkt | Produktname |
| Version | Produktversion |
| islicensed | Produkt ist lizenziert |


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
