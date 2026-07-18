---
title: "AsposePageAbout"
second_title: "Aspose.Page för JavaScript via C++"
description: "Hämta information om produkten."
type: docs
url: /sv/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Hämta information om produkten.

```js
function AsposePageAbout()
```

### Returvärde

JSON-objekt
| Fält | Beskrivning |
| ----- | ----------- |
| errorCode | kodfel (0 inget fel) |
| errorText | textfel ("" inget fel) |
| produkt | Produktnamn |
| version | Produktversion |
| islicensed | Produkten är licensierad |


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
