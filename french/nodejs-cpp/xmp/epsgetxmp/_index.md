---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Obtenir les métadonnées XMP"
type: docs
weight: 10
url: /fr/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Lit le fichier PS/EPS et extrait les métadonnées XMP si elles existent déjà.
Si le fichier EPS ne contient pas de métadonnées XMP, nous obtenons un nouveau fichier rempli avec les valeurs des commentaires de métadonnées PS (%%Creator, %%CreateDate, %%Title, etc.).
Le fichier EPS avec les métadonnées XMP remplies sera enregistré dans fileNameResult.

```js
function AsposeEPSGetXmp(
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
|  | XMP | tableau de valeurs de métadonnées |
|  | fileNameResult | nom du fichier résultat |

### Exemples

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

### Voir aussi

* function [XPSSaveAsImage](../xpssaveasimage/)
