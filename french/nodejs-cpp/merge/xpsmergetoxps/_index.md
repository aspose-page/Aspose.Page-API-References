---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Fusionner les fichiers XPS en un XPS"
type: docs
weight: 10
url: /fr/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Fusionner plusieurs fichiers XPS en un seul fichier XPS.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileNames | string | Les noms des fichiers à fusionner. |
| fileNameResult | string | Le nom du fichier XPS résultant. |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Voir aussi

* function [XPSMergeToPdf](../xpsmergetopdf/)
