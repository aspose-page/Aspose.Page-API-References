---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page för JavaScript via C++"
description: "Hämta XMP-metadata"
type: docs
weight: 10
url: /sv/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Läser PS/EPS-fil och extraherar XmpMetdata om den redan finns.
Om EPS-filen inte innehåller XMP-metadata får vi en ny som fylls med värden från PS-metadata-kommentarer (%%Creator, %%CreateDate, %%Title etc).
EPS‑fil med ifylld XMP‑metadata kommer att sparas i fileNameResult.

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll i källfilen. |
| fileName | string | Källfilens namn. |
| fileNameResult | string | Resultatfilens namn. |


### Returvärde

JSON-objekt
| Fält | Beskrivning |
| ----- | ----------- |
|  | errorCode | kodfel (0 inget fel) |
|  | errorText | textfel ("" inget fel) |
|  | XMP | array av metadatavärden |
|  | fileNameResult | resultatfilnamn |

### Exempel

```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeEPSGetXMP(eps_file, img_file + "_out.eps");
    console.log("AsposeEPSGetXMP => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Se även

* function [XPSSaveAsImage](../xpssaveasimage/)
