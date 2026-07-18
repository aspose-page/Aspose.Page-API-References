---
title: "XPSSaveAsPdf"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "XPS를 PDF로 변환합니다"
type: docs
weight: 10
url: /ko/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

XPS를 PDF로 변환합니다.

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileBlob | Blob 객체 | 변환을 위한 원본 글꼴 내용. |
| fileName | string | 파일 이름. |
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

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsPdf(xps_file,true);
    console.log("XPSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 관련 항목

* function [XPSSaveAsImage](../xpssaveasimage/)
