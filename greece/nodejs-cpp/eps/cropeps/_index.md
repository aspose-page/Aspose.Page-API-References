---
title: "AsposeCropEPS"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Κόψιμο EPS"
type: docs
weight: 10
url: /el/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Κόβει αρχείο EPS. Αποθηκεύει το αρχικό αρχείο EPS με ενημερωμένο υπάρχον %%BoundingBox ή θα δημιουργηθεί νέο.

```js
function AsposeCropEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    left,
    top,
    right,
    bottom
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileBlob | Αντικείμενο Blob | Περιεχόμενο του αρχικού αρχείου. |
| fileName | string | Όνομα αρχείου προέλευσης. |
| fileNameResult | string | Όνομα αρχείου αποτελέσματος. |
| αριστερά | float | Καθορίζει το αριστερό όριο του πλαισίου περικοπής. |
| επάνω | float | Καθορίζει το επάνω όριο του πλαισίου περικοπής. |
| δεξιά | float | Καθορίζει το δεξί όριο του πλαισίου περικοπής. |
| κάτω | float | Καθορίζει το κάτω όριο του πλαισίου περικοπής. |

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

    //CropEPS - working with EPS
    const json = AsposePageModule.AsposeCropEPS(eps_file, "croped.eps", 30, 5, 240, 36);
    console.log("CropEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Δείτε επίσης

* function [AsposeResizeEps](../resizeeps/)
