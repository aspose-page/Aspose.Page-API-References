---
title: "AsposeSaveImageAsEps"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Redimensionner EPS"
type: docs
weight: 10
url: /fr/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

Redimensionne le fichier EPS. Il enregistre le fichier EPS initial avec le %%BoundingBox existant mis à jour ou un nouveau sera créé.

```js
function AsposeSaveImageAsEps(
    fileBlob,
    fileName, 
    fileNameResult
)
```

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileBlob | Objet Blob | Contenu du fichier source. |
| fileName | string | Nom du fichier source. |
| fileNameResult | string | Nom du fichier résultant. |

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

### Voir aussi

