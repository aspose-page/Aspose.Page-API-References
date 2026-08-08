---
title: "AsposeGetXpsPageCount"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "XPS ファイルのページ数を取得する"
type: docs
weight: 10
url: /ja/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

XPS ドキュメントのページ数を取得します。

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileBlob | Blob オブジェクト | ソースファイルの内容。 |
| fileName | string | ソースファイル名。 |

### 戻り値

JSON オブジェクト
| フィールド | 説明 |
| ----- | ----------- |
|  | errorCode | コードエラー (0 エラーなし) |
|  | errorText | テキストエラー ("" エラーなし) |
|  | pageCount | ページ数 |

### 例

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


