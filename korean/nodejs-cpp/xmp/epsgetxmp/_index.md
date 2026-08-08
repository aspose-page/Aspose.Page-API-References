---
title: "AsposeEPSGetXmp"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "XMP 메타데이터 가져오기"
type: docs
weight: 10
url: /ko/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

PS/EPS 파일을 읽고 XmpMetdata가 이미 존재하면 추출합니다.
EPS 파일에 XMP 메타데이터가 없으면 PS 메타데이터 주석(%%Creator, %%CreateDate, %%Title 등)에서 값을 채워 새로운 메타데이터를 생성합니다.
EPS 파일에 채워진 XMP 메타데이터가 fileNameResult에 저장됩니다.

```js
function AsposeEPSGetXmp(
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
|  | XMP | 메타데이터 값 배열 |
|  | fileNameResult | 결과 파일 이름 |

### 예제

```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeEPSGetXMP(eps_file, img_file + "_out.eps");
    console.log("AsposeEPSGetXMP => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 관련 항목

* function [XPSSaveAsImage](../xpssaveasimage/)
