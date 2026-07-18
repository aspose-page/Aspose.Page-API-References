---
title: "AsposePageAbout"
second_title: "Aspose.Page για JavaScript μέσω C++"
description: "Αποκτήστε πληροφορίες για το προϊόν."
type: docs
url: /el/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Αποκτήστε πληροφορίες για το προϊόν.

```js
function AsposePageAbout()
```

### Τιμή επιστροφής

Αντικείμενο JSON
| Πεδίο | Περιγραφή |
| ----- | ----------- |
| errorCode | σφάλμα κώδικα (0 χωρίς σφάλμα) |
| errorText | σφάλμα κειμένου ("" χωρίς σφάλμα) |
| προϊόν | Όνομα προϊόντος |
| έκδοση | Έκδοση προϊόντος |
| islicensed | Το προϊόν είναι αδειοδοτημένο |


```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //PageAbout - Get info about Product
    const json = AsposePageModule.AsposePageAbout();
    console.log("PageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```
