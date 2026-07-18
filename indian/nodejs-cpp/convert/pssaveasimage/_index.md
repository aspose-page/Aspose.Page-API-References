---
title: "PSSaveAsImage"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "Postscript को छवि में परिवर्तित करता है"
type: docs
weight: 10
url: /hi/nodejs-cpp/convert/pssaveasimage/
---
## PSSaveAsImage function

Postscript को छवि में परिवर्तित करता है।

```js
function AsposePSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| पैरामीटर | प्रकार | विवरण |
| --------- | ---- | ----------- |
| fileBlob | Blob ऑब्जेक्ट | रूपांतरण के लिए स्रोत फ़ॉन्ट की सामग्री। |
| fileName | string | फ़ाइल नाम। |
| imageFormat | ImageFormat | परिवर्तित करने के लिए छवि स्वरूप। |
| supressErrors | bool | निर्दिष्ट करता है कि त्रुटियों को दमन किया जाना चाहिए या नहीं। |

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

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSSaveAsImage(ps_file, AsposePageModule.ImageFormat.Png, true);
    console.log("PSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### साथ ही देखें

* function [PSSaveAsPdf](../pssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
