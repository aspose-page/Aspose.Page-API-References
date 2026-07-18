---
title: "AsposeResizeEPS"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "EPS को पुनः आकार दें"
type: docs
weight: 10
url: /hi/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

EPS फ़ाइल को पुनः आकार देता है। यह प्रारंभिक EPS फ़ाइल को अद्यतन मौजूद %%BoundingBox के साथ सहेजता है या नया बनाया जाएगा।

```js
function AsposeResizeEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    width,
    height,
    units
)
```

| पैरामीटर | प्रकार | विवरण |
| --------- | ---- | ----------- |
| fileBlob | Blob ऑब्जेक्ट | स्रोत फ़ाइल की सामग्री। |
| fileName | string | स्रोत फ़ाइल नाम। |
| fileNameResult | string | परिणाम फ़ाइल नाम। |
| width | float | नए बाउंडिंग बॉक्स की चौड़ाई निर्दिष्ट करता है। |
| height | float | नए बाउंडिंग बॉक्स की ऊँचाई निर्दिष्ट करता है। |
| unit | Module.Units | नए आकार के प्रकार को निर्दिष्ट करता है। |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### साथ ही देखें

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
