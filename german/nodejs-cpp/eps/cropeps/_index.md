---
title: "AsposeCropEPS"
second_title: "Aspose.Page für JavaScript über C++"
description: "EPS zuschneiden"
type: docs
weight: 10
url: /de/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Beschneidet EPS-Datei. Sie speichert die ursprüngliche EPS-Datei mit aktualisiertem vorhandenen %%BoundingBox oder es wird ein neuer erstellt.

```js
function AsposeCropEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    left,
    top,
    right,
    bottom
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileBlob | Blob-Objekt | Inhalt der Quelldatei. |
| fileName | string | Name der Quelldatei. |
| fileNameResult | string | Name der Ergebnisdatei. |
| links | float | Gibt die linke Grenze des Beschneidungsrahmens an. |
| oben | float | Gibt die obere Grenze des Beschneidungsrahmens an. |
| rechts | float | Gibt die rechte Grenze des Beschneidungsrahmens an. |
| unten | float | Gibt die untere Grenze des Beschneidungsrahmens an. |

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

const eps_file = "./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //CropEPS - working with EPS
    const json = AsposePageModule.AsposeCropEPS(eps_file, "croped.eps", 30, 5, 240, 36);
    console.log("CropEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [AsposeResizeEps](../resizeeps/)
