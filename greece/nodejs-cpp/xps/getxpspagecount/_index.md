---
title: "AsposeGetXpsPageCount"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Λήψη αριθμού σελίδων σε αρχείο XPS"
type: docs
weight: 10
url: /el/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

Λήψη του αριθμού των σελίδων στο έγγραφο xps.

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --------- | ---- | ----------- |
| fileBlob | Αντικείμενο Blob | Περιεχόμενο του αρχικού αρχείου. |
| fileName | string | Όνομα αρχείου προέλευσης. |

### Τιμή επιστροφής

Αντικείμενο JSON
| Πεδίο | Περιγραφή |
| ----- | ----------- |
|  | errorCode | σφάλμα κώδικα (0 χωρίς σφάλμα) |
|  | errorText | σφάλμα κειμένου ("" χωρίς σφάλμα) |
|  | pageCount | αριθμός σελίδων |

### Παραδείγματα

```js
const AsposePage = require('asposepagenodejs');

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    let json = AsposePageModule.AsposePageAbout();
    console.log("AsposePageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : "error:" + json.errorText);

    //AsposeGetXpsPageCount
    json = AsposePageModule.AsposeGetXpsPageCount(xps_file);
    console.log("AsposeGetXpsPageCount => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```


