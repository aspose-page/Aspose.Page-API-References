---
title: "PSSaveAsImage"
second_title: "Aspose.Page für JavaScript über C++"
description: "Konvertiert das Postscript in ein Bild"
type: docs
weight: 10
url: /de/nodejs-cpp/convert/pssaveasimage/
---
## PSSaveAsImage function

Konvertiert das Postscript in ein Bild.

```js
function AsposePSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileBlob | Blob-Objekt | Inhalt der Quellschriftart für die Konvertierung. |
| fileName | string | Dateiname. |
| imageFormat | ImageFormat | Bildformat, in das konvertiert werden soll. |
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

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSSaveAsImage(ps_file, AsposePageModule.ImageFormat.Png, true);
    console.log("PSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [PSSaveAsPdf](../pssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
