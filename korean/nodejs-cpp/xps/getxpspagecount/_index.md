---
title: "AsposeGetXpsPageCount"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "XPS 파일의 페이지 수 가져오기"
type: docs
weight: 10
url: /ko/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

xps 문서의 페이지 수를 가져옵니다.

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| 매개변수 | 유형 | 설명 |
| --------- | ---- | ----------- |
| fileBlob | Blob 객체 | 소스 파일의 내용. |
| fileName | string | 소스 파일 이름. |

### 반환 값

JSON 객체
| 필드 | 설명 |
| ----- | ----------- |
|  | errorCode | 코드 오류 (0 오류 없음) |
|  | errorText | 텍스트 오류 ("" 오류 없음) |
|  | pageCount | 페이지 수 |

### 예제

```js
const AsposePage = require('asposepagenodejs');

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    let json = AsposePageModule.AsposePageAbout();
    console.log("AsposePageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : "error:" + json.errorText);

    //AsposeGetXpsPageCount
    json = AsposePageModule.AsposeGetXpsPageCount(xps_file);
    console.log("AsposeGetXpsPageCount => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```


