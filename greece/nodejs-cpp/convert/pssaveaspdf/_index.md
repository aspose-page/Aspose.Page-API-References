---
title: "PSSaveAsPdf"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Μετατρέπει το Postscript σε PDF"
type: docs
weight: 10
url: /el/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Μετατρέπει το Postscript σε PDF.

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileBlob | Αντικείμενο Blob | Περιεχόμενο της πηγαίας γραμματοσειράς για μετατροπή. |
| fileName | string | Όνομα αρχείου. |
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page για Node.js μέσω παραδειγμάτων C++.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Το άγνωστο σφάλμα έχει εμφανιστεί: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
