---
title: "AsposeResizeEPS"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Redimensionner EPS"
type: docs
weight: 10
url: /fr/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Redimensionne le fichier EPS. Il enregistre le fichier EPS initial avec le %%BoundingBox existant mis à jour ou un nouveau sera créé.

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

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileBlob | Objet Blob | Contenu du fichier source. |
| fileName | string | Nom du fichier source. |
| fileNameResult | string | Nom du fichier résultant. |
| width | float | Spécifie la largeur du nouveau cadre de délimitation. |
| height | float | Spécifie la hauteur du nouveau cadre de délimitation. |
| unit | Module.Units | Spécifie le type de la nouvelle taille. |

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

### Voir aussi

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
