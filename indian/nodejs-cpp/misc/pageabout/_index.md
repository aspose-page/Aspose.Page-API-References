---
title: "AsposePageAbout"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "उत्पाद के बारे में जानकारी प्राप्त करें।"
type: docs
url: /hi/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

उत्पाद के बारे में जानकारी प्राप्त करें।

```js
function AsposePageAbout()
```

### रिटर्न मान

JSON ऑब्जेक्ट
| फ़ील्ड | विवरण |
| ----- | ----------- |
| errorCode | कोड त्रुटि (0 कोई त्रुटि नहीं) |
| errorText | पाठ त्रुटि (\"\" कोई त्रुटि नहीं) |
| उत्पाद | उत्पाद नाम |
| संस्करण | उत्पाद संस्करण |
| islicensed | उत्पाद लाइसेंस प्राप्त है |


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
