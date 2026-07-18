---
title: "AsposeCropEPS"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "क्रॉप EPS"
type: docs
weight: 10
url: /hi/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

EPS फ़ाइल को क्रॉप करता है। यह प्रारंभिक EPS फ़ाइल को अद्यतन मौजूद %%BoundingBox के साथ सहेजता है या नया बनाया जाएगा।

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

| पैरामीटर | प्रकार | विवरण |
| --------- | ---- | ----------- |
| fileBlob | Blob ऑब्जेक्ट | स्रोत फ़ाइल की सामग्री। |
| fileName | string | स्रोत फ़ाइल नाम। |
| fileNameResult | string | परिणाम फ़ाइल नाम। |
| बायाँ | float | क्रॉप बॉक्स की बायीं सीमा निर्दिष्ट करता है। |
| ऊपर | float | क्रॉप बॉक्स की ऊपरी सीमा निर्दिष्ट करता है। |
| दायाँ | float | क्रॉप बॉक्स की दायीं सीमा निर्दिष्ट करता है। |
| नीचे | float | क्रॉप बॉक्स की निचली सीमा निर्दिष्ट करता है। |

### रिटर्न वैल्यू

JSON ऑब्जेक्ट
| फ़ील्ड | विवरण |
| ----- | ----------- |
|  | errorCode | कोड त्रुटि (0 कोई त्रुटि नहीं) |
|  | errorText | पाठ त्रुटि (\"\" कोई त्रुटि नहीं) |
|  | fileNameResult | परिणाम फ़ाइल नाम |

### उदाहरण

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

### साथ ही देखें

* function [AsposeResizeEps](../resizeeps/)
