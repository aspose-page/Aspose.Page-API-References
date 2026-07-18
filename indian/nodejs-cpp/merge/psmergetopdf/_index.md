---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page जावास्क्रिप्ट के लिए C++ के माध्यम से"
description: "Postscript फ़ाइलों को PDF में मिलाएँ"
type: docs
weight: 10
url: /hi/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Postscript फ़ाइलों को PDF में मिलाएँ।

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| पैरामीटर | प्रकार | विवरण |
| --------- | ---- | ----------- |
| fileNames | string | मर्ज के लिए फ़ाइलों के नाम। |
| fileNameResult | string | परिणाम PDF फ़ाइल का नाम। |
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### साथ ही देखें

* function [PSSaveAsImage](../pssaveasimage/)
