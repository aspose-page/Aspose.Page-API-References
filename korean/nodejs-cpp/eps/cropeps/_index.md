---
title: "AsposeCropEPS"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "EPS 자르기"
type: docs
weight: 10
url: /ko/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

EPS 파일을 자릅니다. 기존 %%BoundingBox를 업데이트한 초기 EPS 파일을 저장하거나 새 파일이 생성됩니다.

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

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileBlob | Blob 객체 | 소스 파일의 내용. |
| fileName | string | 소스 파일 이름. |
| fileNameResult | string | 결과 파일 이름. |
| 왼쪽 | float | 자르기 상자의 왼쪽 경계를 지정합니다. |
| 위쪽 | float | 자르기 상자의 위쪽 경계를 지정합니다. |
| 오른쪽 | float | 자르기 상자의 오른쪽 경계를 지정합니다. |
| 아래쪽 | float | 자르기 상자의 아래쪽 경계를 지정합니다. |

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

### 관련 항목

* function [AsposeResizeEps](../resizeeps/)
