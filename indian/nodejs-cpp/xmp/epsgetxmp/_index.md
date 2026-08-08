---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "XMP मेटाडेटा प्राप्त करें"
type: docs
weight: 10
url: /hi/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

PS/EPS फ़ाइल को पढ़ता है और यदि XMP मेटाडेटा पहले से मौजूद है तो उसे निकालता है।
यदि EPS फ़ाइल में XMP मेटाडेटा नहीं है तो हम एक नया मेटाडेटा प्राप्त करते हैं जो PS मेटाडेटा टिप्पणियों (%%Creator, %%CreateDate, %%Title आदि) से मानों से भरा होता है।
EPS फ़ाइल जिसमें भरा हुआ XMP मेटाडेटा है, fileNameResult में सहेजी जाएगी।

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| पैरामीटर | प्रकार | विवरण |
| --------- | ---- | ----------- |
| fileBlob | Blob ऑब्जेक्ट | स्रोत फ़ाइल की सामग्री। |
| fileName | string | स्रोत फ़ाइल नाम। |
| fileNameResult | string | परिणाम फ़ाइल नाम। |


### रिटर्न वैल्यू

JSON ऑब्जेक्ट
| फ़ील्ड | विवरण |
| ----- | ----------- |
|  | errorCode | कोड त्रुटि (0 कोई त्रुटि नहीं) |
|  | errorText | पाठ त्रुटि (\"\" कोई त्रुटि नहीं) |
|  | XMP | मेटाडेटा मानों की सरणी |
|  | fileNameResult | परिणाम फ़ाइल नाम |

### उदाहरण

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

### साथ ही देखें

* function [XPSSaveAsImage](../xpssaveasimage/)
