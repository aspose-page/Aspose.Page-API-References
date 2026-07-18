---
title: "XPSSaveAsImage"
second_title: "Aspose.Page für JavaScript über C++"
description: "Konvertiert das XPS in ein Bild"
type: docs
weight: 10
url: /de/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Konvertiert das Postscript in ein Bild.

```js
function AsposeXPSSaveAsImage(
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

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
