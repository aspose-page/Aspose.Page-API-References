---
title: "XPSSaveAsImage"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Μετατρέπει το XPS σε εικόνα"
type: docs
weight: 10
url: /el/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Μετατρέπει το Postscript σε εικόνα.

```js
function AsposeXPSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileBlob | Αντικείμενο Blob | Περιεχόμενο της πηγαίας γραμματοσειράς για μετατροπή. |
| fileName | string | Όνομα αρχείου. |
| imageFormat | ImageFormat | μορφή εικόνας για μετατροπή. |
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

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Δείτε επίσης

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
