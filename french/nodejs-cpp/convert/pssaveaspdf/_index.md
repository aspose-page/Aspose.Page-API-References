---
title: "PSSaveAsPdf"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Convertit le Postscript en PDF"
type: docs
weight: 10
url: /fr/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Convertit le Postscript en PDF.

```js
function AsposePSSaveAsPdf(
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`L'erreur inconnue s'est produite : ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
