---
title: "XPSSaveAsImage"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "XPS を画像に変換します"
type: docs
weight: 10
url: /ja/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Postscript を画像に変換します。

```js
function AsposeXPSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileBlob | Blob オブジェクト | 変換用のソースフォントの内容です。 |
| fileName | string | ファイル名。 |
| imageFormat | ImageFormat | 変換する画像形式。 |
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

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 関連項目

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
