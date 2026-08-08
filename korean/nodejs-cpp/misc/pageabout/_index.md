---
title: "AsposePageAbout"
second_title: "C++를 통한 JavaScript용 Aspose.Page"
description: "제품에 대한 정보를 가져옵니다."
type: docs
url: /ko/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

제품에 대한 정보를 가져옵니다.

```js
function AsposePageAbout()
```

### 반환 값

JSON 객체
| 필드 | 설명 |
| ----- | ----------- |
| errorCode | 코드 오류 (0 오류 없음) |
| errorText | 텍스트 오류 ("" 오류 없음) |
| 제품 | 제품 이름 |
| 버전 | 제품 버전 |
| islicensed | 제품에 라이선스가 부여되었습니다. |


```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //PageAbout - Get info about Product
    const json = AsposePageModule.AsposePageAbout();
    console.log("PageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```
