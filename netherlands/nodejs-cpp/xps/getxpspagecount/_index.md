---
title: "AsposeGetXpsPageCount"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Aantal pagina's in XPS-bestand ophalen"
type: docs
weight: 10
url: /nl/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

Haal het aantal pagina's op in het xps-document.

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van bronbestand. |
| fileName | string | Naam van bronbestand. |

### Retourwaarde

JSON-object
| Veld | Beschrijving |
| ----- | ----------- |
|  | errorCode | codefout (0 geen fout) |
|  | errorText | tekstfout ("" geen fout) |
|  | pageCount | aantal pagina's |

### Voorbeelden

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


