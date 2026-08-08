---
title: "AsposePageAbout"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Haal informatie op over Product."
type: docs
url: /nl/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Haal informatie op over Product.

```js
function AsposePageAbout()
```

### Retourwaarde

JSON-object
| Veld | Beschrijving |
| ----- | ----------- |
| errorCode | codefout (0 geen fout) |
| errorText | tekstfout ("" geen fout) |
| product | Productnaam |
| versie | Productversie |
| islicensed | Product is gelicentieerd |


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
