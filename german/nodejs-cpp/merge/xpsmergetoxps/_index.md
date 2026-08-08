---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page für JavaScript über C++"
description: "XPS-Dateien zu einer XPS zusammenführen"
type: docs
weight: 10
url: /de/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Mehrere XPS-Dateien zu einer XPS-Datei zusammenführen.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileNames | string | Die Namen der Dateien zum Zusammenführen. |
| fileNameResult | string | Der Name der Ergebnis-XPS-Datei. |
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

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [XPSMergeToPdf](../xpsmergetopdf/)
