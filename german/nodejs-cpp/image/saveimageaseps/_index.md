---
title: "AsposeSaveImageAsEps"
second_title: "Aspose.Page für JavaScript über C++"
description: "EPS skalieren"
type: docs
weight: 10
url: /de/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

Skaliert EPS-Datei. Sie speichert die ursprüngliche EPS-Datei mit aktualisiertem vorhandenen %%BoundingBox, oder es wird ein neuer erstellt.

```js
function AsposeSaveImageAsEps(
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
|  | fileNameResult | Ergebnisdateiname |

### Beispiele

```js
const AsposePage = require('asposepagenodejs');

const img_file = "./data/PAGENET-361-10.bmp";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //SaveImageAsEps - convert image to EPS
    const json = AsposePageModule.AsposeSaveImageAsEps(img_file, img_file + ".eps");
    console.log("SaveImageAsEps => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

