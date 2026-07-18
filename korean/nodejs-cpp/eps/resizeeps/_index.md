---
title: "AsposeResizeEPS"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "EPS 크기 조정"
type: docs
weight: 10
url: /ko/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

EPS 파일의 크기를 조정합니다. 기존 %%BoundingBox를 업데이트하거나 새로 생성된 %%BoundingBox와 함께 초기 EPS 파일을 저장합니다.

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

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileBlob | Blob 객체 | 소스 파일의 내용. |
| fileName | string | 소스 파일 이름. |
| fileNameResult | string | 결과 파일 이름. |
| width | float | 새 경계 상자의 너비를 지정합니다. |
| height | float | 새 경계 상자의 높이를 지정합니다. |
| unit | Module.Units | 새 크기의 유형을 지정합니다. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 관련 항목

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
