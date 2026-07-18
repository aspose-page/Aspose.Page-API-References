---
title: "AsposeSaveImageAsEps"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "EPS को पुनः आकार दें"
type: docs
weight: 10
url: /hi/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

EPS फ़ाइल को पुनः आकार देता है। यह प्रारंभिक EPS फ़ाइल को अद्यतन मौजूद %%BoundingBox के साथ सहेजता है या नया बनाया जाएगा।

```js
function AsposeSaveImageAsEps(
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
|  | fileNameResult | परिणाम फ़ाइल नाम |

### उदाहरण

```js
const AsposePage = require('asposepagenodejs');

const img_file = "./data/PAGENET-361-10.bmp";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //SaveImageAsEps - convert image to EPS
    const json = AsposePageModule.AsposeSaveImageAsEps(img_file, img_file + ".eps");
    console.log("SaveImageAsEps => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### साथ ही देखें

