---
title: "AsposeResizeEPS"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Αλλαγή μεγέθους EPS"
type: docs
weight: 10
url: /el/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Αλλάζει το μέγεθος του αρχείου EPS. Αποθηκεύει το αρχικό αρχείο EPS με ενημερωμένο υπάρχον %%BoundingBox ή δημιουργείται νέο.

```js
function AsposeResizeEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    width,
    height,
    units
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileBlob | Αντικείμενο Blob | Περιεχόμενο του αρχικού αρχείου. |
| fileName | string | Όνομα αρχείου προέλευσης. |
| fileNameResult | string | Όνομα αρχείου αποτελέσματος. |
| width | float | Καθορίζει το πλάτος του νέου bounding box. |
| height | float | Καθορίζει το ύψος του νέου bounding box. |
| unit | Module.Units | Καθορίζει τον τύπο του νέου μεγέθους. |

### Τιμή επιστροφής

Αντικείμενο JSON
| Πεδίο | Περιγραφή |
| ----- | ----------- |
|  | errorCode | σφάλμα κώδικα (0 χωρίς σφάλμα) |
|  | errorText | σφάλμα κειμένου ("" χωρίς σφάλμα) |
|  | fileNameResult | όνομα αρχείου αποτελέσματος |

### Παραδείγματα

```js
const AsposePage = require('asposepagenodejs');

const eps_file = "./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Δείτε επίσης

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
