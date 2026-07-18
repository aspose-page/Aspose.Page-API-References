---
title: "AsposePageAbout"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Obtenir des informations sur le produit."
type: docs
url: /fr/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Obtenir des informations sur le produit.

```js
function AsposePageAbout()
```

### Valeur de retour

Objet JSON
| Champ | Description |
| ----- | ----------- |
| errorCode | erreur de code (0 aucune erreur) |
| errorText | erreur de texte ("" aucune erreur) |
| produit | Nom du produit |
| version | Version du produit |
| islicensed | Le produit est licencié |


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
