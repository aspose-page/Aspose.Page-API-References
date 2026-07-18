---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Fusionner les fichiers Postscript en PDF"
type: docs
weight: 10
url: /fr/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Fusionner les fichiers Postscript en PDF.

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileNames | string | Les noms des fichiers à fusionner. |
| fileNameResult | string | Le nom du fichier PDF résultant. |
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Voir aussi

* function [PSSaveAsImage](../pssaveasimage/)
