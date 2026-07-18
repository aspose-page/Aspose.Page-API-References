---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page voor JavaScript via C++"
description: "Voeg de XPS-bestanden samen tot één XPS"
type: docs
weight: 10
url: /nl/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Voeg de verschillende XPS-bestanden samen tot één XPS-bestand.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Type | Beschrijving |
| --------- | ---- | ----------- |
| fileNames | string | De namen van bestanden voor samenvoegen. |
| fileNameResult | string | De naam van het resulterende xps-bestand. |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Zie ook

* function [XPSMergeToPdf](../xpsmergetopdf/)
