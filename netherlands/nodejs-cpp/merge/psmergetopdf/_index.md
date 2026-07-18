---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Voeg de Postscript-bestanden samen tot PDF"
type: docs
weight: 10
url: /nl/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Voeg de Postscript-bestanden samen tot PDF.

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileNames | string | De namen van bestanden voor samenvoegen. |
| fileNameResult | string | De naam van het resulterende pdf-bestand. |
| supressErrors | bool | Specificeert of fouten al dan niet onderdrukt moeten worden. |

### Retourwaarde

JSON-object
| Veld | Beschrijving |
| ----- | ----------- |
|  | errorCode | codefout (0 geen fout) |
|  | errorText | tekstfout ("" geen fout) |
|  | fileNameResult | resultaat bestandsnaam |

### Voorbeelden

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

### Zie ook

* function [PSSaveAsImage](../pssaveasimage/)
