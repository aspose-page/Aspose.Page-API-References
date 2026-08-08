---
title: "AsposeResizeEPS"
second_title: "Aspose.Page für JavaScript über C++"
description: "EPS skalieren"
type: docs
weight: 10
url: /de/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Skaliert EPS-Datei. Sie speichert die ursprüngliche EPS-Datei mit aktualisiertem vorhandenen %%BoundingBox, oder es wird ein neuer erstellt.

```js
function AsposeResizeEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    width,
    height,
    units
)
```

| Parameter | Typ | Beschreibung |
| --------- | ---- | ----------- |
| fileBlob | Blob-Objekt | Inhalt der Quelldatei. |
| fileName | string | Name der Quelldatei. |
| fileNameResult | string | Name der Ergebnisdatei. |
| Breite | float | Gibt die Breite des neuen Begrenzungsrahmens an. |
| Höhe | float | Gibt die Höhe des neuen Begrenzungsrahmens an. |
| Einheit | Module.Units | Gibt den Typ der neuen Größe an. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Siehe auch

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
