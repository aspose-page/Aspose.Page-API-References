---
title: "XPSSaveAsPdf"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "XPS を PDF に変換します"
type: docs
weight: 10
url: /ja/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

XPS を PDF に変換します。

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileBlob | Blob オブジェクト | 変換用のソースフォントの内容です。 |
| fileName | string | ファイル名。 |
| supressErrors | bool | エラーを抑制するかどうかを指定します。 |

### 戻り値

JSON オブジェクト
| フィールド | 説明 |
| ----- | ----------- |
|  | errorCode | コードエラー (0 エラーなし) |
|  | errorText | テキストエラー ("" エラーなし) |
|  | fileNameResult | 結果ファイル名 |

### 例

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

### 関連項目

* function [XPSSaveAsImage](../xpssaveasimage/)
