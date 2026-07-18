---
title: "XPSSaveAsPdf"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Convertit le XPS en PDF"
type: docs
weight: 10
url: /fr/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

Convertit le XPS en PDF.

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileBlob | Objet Blob | Contenu de la police source pour la conversion. |
| fileName | string | Nom du fichier. |
| supressErrors | bool | Spécifie si les erreurs doivent être supprimées ou non. |

### Valeur de retour

Objet JSON
| Champ | Description |
| ----- | ----------- |
|  | errorCode | erreur de code (0 aucune erreur) |
|  | errorText | erreur de texte ("" aucune erreur) |
|  | fileNameResult | nom du fichier résultat |

### Exemples

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

### Voir aussi

* function [XPSSaveAsImage](../xpssaveasimage/)
