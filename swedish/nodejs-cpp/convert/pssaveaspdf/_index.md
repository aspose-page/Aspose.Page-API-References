---
title: "PSSaveAsPdf"
second_title: "Aspose.Page för JavaScript via C++"
description: "Konverterar Postscript till PDF"
type: docs
weight: 10
url: /sv/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Konverterar Postscript till PDF.

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileBlob | Blob-objekt | Innehåll för källteckensnitt för konvertering. |
| fileName | string | Filnamn. |
| supressErrors | bool | Anger om fel ska undertryckas eller inte. |

### Returvärde

JSON-objekt
| Fält | Beskrivning |
| ----- | ----------- |
|  | errorCode | kodfel (0 inget fel) |
|  | errorText | textfel ("" inget fel) |
|  | fileNameResult | resultatfilnamn |

### Exempel

```js
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page för Node.js via C++-exempel.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Det okända felet har inträffat: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
