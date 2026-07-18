---
title: "AsposeSaveImageAsEps"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "EPS 크기 조정"
type: docs
weight: 10
url: /ko/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

EPS 파일의 크기를 조정합니다. 기존 %%BoundingBox를 업데이트하거나 새로 생성된 %%BoundingBox와 함께 초기 EPS 파일을 저장합니다.

```js
function AsposeSaveImageAsEps(
    fileBlob,
    fileName, 
    fileNameResult
)
```

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileBlob | Blob 객체 | 소스 파일의 내용. |
| fileName | string | 소스 파일 이름. |
| fileNameResult | string | 결과 파일 이름. |

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

### 관련 항목

