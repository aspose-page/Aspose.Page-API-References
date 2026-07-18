---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page för JavaScript via C++"
description: "Sammanfoga Postscript-filerna till PDF"
type: docs
weight: 10
url: /sv/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Sammanfoga Postscript-filerna till PDF.

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileNames | string | Namnen på filer för sammanslagning. |
| fileNameResult | string | Namnet på den resulterande pdf-filen. |
| supressErrors | bool | Anger om fel ska undertryckas eller inte. |

### Returvärde

JSON-objekt
| Fält | Beskrivning |
| ----- | ----------- |
|  | errorCode | kodfel (0 inget fel) |
|  | errorText | textfel ("" inget fel) |
|  | fileNameResult | resultatfilnamn |

### Exempel

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

### Se även

* function [PSSaveAsImage](../pssaveasimage/)
