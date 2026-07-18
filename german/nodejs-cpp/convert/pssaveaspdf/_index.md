---
title: "PSSaveAsPdf"
second_title: "Aspose.Page für JavaScript über C++"
description: "Konvertiert das Postscript zu PDF"
type: docs
weight: 10
url: /de/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Konvertiert das Postscript zu PDF.

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileBlob | Blob-Objekt | Inhalt der Quellschriftart für die Konvertierung. |
| fileName | string | Dateiname. |
| supressErrors | bool | Gibt an, ob Fehler unterdrückt werden sollen oder nicht. |

### Rückgabewert

JSON-Objekt
| Feld | Beschreibung |
| ----- | ----------- |
|  | errorCode | Code-Fehler (0 kein Fehler) |
|  | errorText | Textfehler ("" kein Fehler) |
|  | fileNameResult | Ergebnisdateiname |

### Beispiele

```js
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page für Node.js über C++-Beispiele.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Der unbekannte Fehler ist aufgetreten: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
