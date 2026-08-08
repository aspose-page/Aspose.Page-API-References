---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Λήψη μεταδεδομένων XMP"
type: docs
weight: 10
url: /el/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Διαβάζει αρχείο PS/EPS και εξάγει τα μεταδεδομένα XmpMetdata εάν υπάρχουν ήδη.
Εάν το αρχείο EPS δεν περιέχει μεταδεδομένα XMP, δημιουργούμε ένα νέο γεμάτο με τιμές από τα σχόλια μεταδεδομένων PS (%%Creator, %%CreateDate, %%Title κλ.).
Το αρχείο EPS με συμπληρωμένα μεταδεδομένα XMP θα αποθηκευτεί στο fileNameResult.

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileBlob | Αντικείμενο Blob | Περιεχόμενο του αρχικού αρχείου. |
| fileName | string | Όνομα αρχείου προέλευσης. |
| fileNameResult | string | Όνομα αρχείου αποτελέσματος. |


### Τιμή επιστροφής

Αντικείμενο JSON
| Πεδίο | Περιγραφή |
| ----- | ----------- |
|  | errorCode | σφάλμα κώδικα (0 χωρίς σφάλμα) |
|  | errorText | σφάλμα κειμένου ("" χωρίς σφάλμα) |
|  | XMP | πίνακας τιμών μεταδεδομένων |
|  | fileNameResult | όνομα αρχείου αποτελέσματος |

### Παραδείγματα

```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeEPSGetXMP(eps_file, img_file + "_out.eps");
    console.log("AsposeEPSGetXMP => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Δείτε επίσης

* function [XPSSaveAsImage](../xpssaveasimage/)
