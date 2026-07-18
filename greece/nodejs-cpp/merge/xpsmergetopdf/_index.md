---
title: "AsposeXPSMergeToPdf"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Συγχώνευση των αρχείων XPS σε PDF"
type: docs
weight: 10
url: /el/nodejs-cpp/merge/xpsmergetopdf/
---
## AsposeXPSMergeToPdf function

Συγχώνευση των αρχείων XPS σε PDF.

```js
function AsposeXPSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileNames | string | Τα ονόματα των αρχείων για συγχώνευση. |
| fileNameResult | string | Το όνομα του τελικού αρχείου pdf. |
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

    const json = AsposePageModule.AsposeXPSMergeToPdf(xps_files,"XPsMergedToPdfResult.pdf");
    console.log("XPSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Δείτε επίσης

* function [PSSaveAsImage](../pssaveasimage/)
