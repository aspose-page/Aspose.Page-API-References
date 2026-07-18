---
title: "PSSaveAsPdf"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "Postscript को PDF में परिवर्तित करता है"
type: docs
weight: 10
url: /hi/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Postscript को PDF में परिवर्तित करता है।

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| पैरामीटर | प्रकार | विवरण |
| --------- | ---- | ----------- |
| fileBlob | Blob ऑब्जेक्ट | रूपांतरण के लिए स्रोत फ़ॉन्ट की सामग्री। |
| fileName | string | फ़ाइल नाम। |
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page के लिए Node.js के माध्यम से C++ उदाहरण।");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`अज्ञात त्रुटि उत्पन्न हुई है: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
