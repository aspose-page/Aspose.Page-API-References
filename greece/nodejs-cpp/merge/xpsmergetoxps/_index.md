---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Συγχώνευση των αρχείων XPS σε ένα XPS"
type: docs
weight: 10
url: /el/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Συγχώνευση πολλών αρχείων XPS σε ένα αρχείο XPS.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileNames | string | Τα ονόματα των αρχείων για συγχώνευση. |
| fileNameResult | string | Το όνομα του τελικού αρχείου xps. |
| supressErrors | bool | Καθορίζει εάν τα σφάλματα πρέπει να καταστέλλονται ή όχι. |

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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Δείτε επίσης

* function [XPSMergeToPdf](../xpsmergetopdf/)
