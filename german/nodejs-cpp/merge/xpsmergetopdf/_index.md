---
title: "AsposeXPSMergeToPdf"
second_title: "Aspose.Page für JavaScript über C++"
description: "XPS-Dateien zu PDF zusammenführen"
type: docs
weight: 10
url: /de/nodejs-cpp/merge/xpsmergetopdf/
---
## AsposeXPSMergeToPdf function

XPS-Dateien zu PDF zusammenführen.

```js
function AsposeXPSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileNames | string | Die Namen der Dateien zum Zusammenführen. |
| fileNameResult | string | Der Name der Ergebnis-PDF-Datei. |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToPdf(xps_files,"XPsMergedToPdfResult.pdf");
    console.log("XPSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [PSSaveAsImage](../pssaveasimage/)
