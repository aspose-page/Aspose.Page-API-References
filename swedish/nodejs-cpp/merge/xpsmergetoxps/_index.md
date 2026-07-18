---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page för JavaScript via C++"
description: "Sammanfoga XPS-filerna till en XPS"
type: docs
weight: 10
url: /sv/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Sammanfoga flera XPS-filer till en XPS-fil.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Typ | Beskrivning |
| --------- | ---- | ----------- |
| fileNames | string | Namnen på filer för sammanslagning. |
| fileNameResult | string | Namnet på den resulterande xps-filen. |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Se även

* function [XPSMergeToPdf](../xpsmergetopdf/)
