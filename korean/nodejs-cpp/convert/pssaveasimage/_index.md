---
title: "PSSaveAsImage"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "Postscript를 이미지로 변환합니다"
type: docs
weight: 10
url: /ko/nodejs-cpp/convert/pssaveasimage/
---
## PSSaveAsImage function

Postscript를 이미지로 변환합니다.

```js
function AsposePSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileBlob | Blob 객체 | 변환을 위한 원본 글꼴 내용. |
| fileName | string | 파일 이름. |
| imageFormat | ImageFormat | 변환할 이미지 형식. |
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

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSSaveAsImage(ps_file, AsposePageModule.ImageFormat.Png, true);
    console.log("PSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 관련 항목

* function [PSSaveAsPdf](../pssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
