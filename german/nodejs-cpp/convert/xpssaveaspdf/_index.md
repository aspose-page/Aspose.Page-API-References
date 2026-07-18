---
title: "XPSSaveAsPdf"
second_title: "Aspose.Page für JavaScript über C++"
description: "Konvertiert das XPS in ein PDF"
type: docs
weight: 10
url: /de/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

Konvertiert das XPS in ein PDF.

```js
function AsposeXPSSaveAsPdf(
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
const AsposePage = require('asposepagenodejs');

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsPdf(xps_file,true);
    console.log("XPSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [XPSSaveAsImage](../xpssaveasimage/)
