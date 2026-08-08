---
title: "AsposeCropEPS"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Recadrer EPS"
type: docs
weight: 10
url: /fr/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Recadre le fichier EPS. Il enregistre le fichier EPS initial avec le %%BoundingBox existant mis à jour ou un nouveau sera créé.

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

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileBlob | Objet Blob | Contenu du fichier source. |
| fileName | string | Nom du fichier source. |
| fileNameResult | string | Nom du fichier résultant. |
| gauche | float | Spécifie la limite gauche de la boîte de recadrage. |
| haut | float | Spécifie la limite supérieure de la boîte de recadrage. |
| droite | float | Spécifie la limite droite de la boîte de recadrage. |
| bas | float | Spécifie la limite inférieure de la boîte de recadrage. |

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

    //CropEPS - working with EPS
    const json = AsposePageModule.AsposeCropEPS(eps_file, "croped.eps", 30, 5, 240, 36);
    console.log("CropEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Voir aussi

* function [AsposeResizeEps](../resizeeps/)
