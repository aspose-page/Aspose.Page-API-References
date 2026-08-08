---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page für JavaScript über C++"
description: "XMP-Metadaten abrufen"
type: docs
weight: 10
url: /de/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Liest PS/EPS-Datei und extrahiert XmpMetdata, falls sie bereits vorhanden sind.
Wenn die EPS-Datei keine XMP-Metadaten enthält, erhalten wir neue, die mit Werten aus den PS-Metadatenkommentaren (%%Creator, %%CreateDate, %%Title usw.) gefüllt sind.
EPS-Datei mit ausgefüllten XMP-Metadaten wird in fileNameResult gespeichert.

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileBlob | Blob-Objekt | Inhalt der Quelldatei. |
| fileName | string | Name der Quelldatei. |
| fileNameResult | string | Name der Ergebnisdatei. |


### Rückgabewert

JSON-Objekt
| Feld | Beschreibung |
| ----- | ----------- |
|  | errorCode | Code-Fehler (0 kein Fehler) |
|  | errorText | Textfehler ("" kein Fehler) |
|  | XMP | Array von Metadatenwerten |
|  | fileNameResult | Ergebnisdateiname |

### Beispiele

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

### Siehe auch

* function [XPSSaveAsImage](../xpssaveasimage/)
