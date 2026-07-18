---
title: "AsposePageAbout"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "製品に関する情報を取得します。"
type: docs
url: /ja/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

製品に関する情報を取得します。

```js
function AsposePageAbout()
```

### 戻り値

JSON オブジェクト
| フィールド | 説明 |
| ----- | ----------- |
| errorCode | コードエラー (0 エラーなし) |
| errorText | テキストエラー ("" エラーなし) |
| 製品 | 製品名 |
| バージョン | 製品バージョン |
| islicensed | 製品はライセンスされています |


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
