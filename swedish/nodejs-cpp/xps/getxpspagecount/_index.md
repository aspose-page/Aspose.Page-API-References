---
title: "AsposeGetXpsPageCount"
second_title: "Aspose.Page för JavaScript via C++"
description: "Hämta antal sidor i XPS-fil"
type: docs
weight: 10
url: /sv/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

Hämta antalet sidor i xps-dokumentet.

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll i källfilen. |
| fileName | string | Källfilens namn. |

### Returvärde

JSON-objekt
| Fält | Beskrivning |
| ----- | ----------- |
|  | errorCode | kodfel (0 inget fel) |
|  | errorText | textfel ("" inget fel) |
|  | pageCount | antal sidor |

### Exempel

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


