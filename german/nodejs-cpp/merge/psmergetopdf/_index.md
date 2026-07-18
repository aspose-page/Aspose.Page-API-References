---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page für JavaScript über C++"
description: "Postscript-Dateien zu PDF zusammenführen"
type: docs
weight: 10
url: /de/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Postscript-Dateien zu PDF zusammenführen.

```js
function AsposePSMergePdf(
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [PSSaveAsImage](../pssaveasimage/)
