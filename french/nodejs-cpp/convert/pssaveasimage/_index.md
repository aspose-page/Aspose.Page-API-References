---
title: "PSSaveAsImage"
second_title: "Aspose.Page pour JavaScript via C++"
description: "Convertit le Postscript en image"
type: docs
weight: 10
url: /fr/nodejs-cpp/convert/pssaveasimage/
---
## PSSaveAsImage function

Convertit le Postscript en image.

```js
function AsposePSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
| fileBlob | Objet Blob | Contenu de la police source pour la conversion. |
| fileName | string | Nom du fichier. |
| imageFormat | ImageFormat | format d'image dans lequel convertir. |
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

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSSaveAsImage(ps_file, AsposePageModule.ImageFormat.Png, true);
    console.log("PSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Voir aussi

* function [PSSaveAsPdf](../pssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
