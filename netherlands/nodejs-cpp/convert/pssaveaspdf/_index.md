---
title: "PSSaveAsPdf"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Converteert de Postscript naar PDF"
type: docs
weight: 10
url: /nl/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Converteert de Postscript naar PDF.

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileBlob | Blob-object | Inhoud van het bronlettertype voor conversie. |
| fileName | string | Bestandsnaam. |
| supressErrors | bool | Specificeert of fouten al dan niet onderdrukt moeten worden. |

### Retourwaarde

JSON-object
| Veld | Beschrijving |
| ----- | ----------- |
|  | errorCode | codefout (0 geen fout) |
|  | errorText | tekstfout ("" geen fout) |
|  | fileNameResult | resultaat bestandsnaam |

### Voorbeelden

```js
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page voor Node.js via C++ voorbeelden.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Er is een onbekende fout opgetreden: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
