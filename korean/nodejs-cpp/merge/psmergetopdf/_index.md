---
title: "AsposePSMergeToPdf"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "Postscript 파일을 PDF로 병합합니다"
type: docs
weight: 10
url: /ko/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Postscript 파일을 PDF로 병합합니다.

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileNames | string | 병합을 위한 파일 이름들. |
| fileNameResult | string | 결과 PDF 파일의 이름입니다. |
| supressErrors | bool | 오류를 억제해야 하는지 여부를 지정합니다. |

### 반환 값

JSON 객체
| 필드 | 설명 |
| ----- | ----------- |
|  | errorCode | 코드 오류 (0 오류 없음) |
|  | errorText | 텍스트 오류 ("" 오류 없음) |
|  | fileNameResult | 결과 파일 이름 |

### 예제

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

### 관련 항목

* function [PSSaveAsImage](../pssaveasimage/)
