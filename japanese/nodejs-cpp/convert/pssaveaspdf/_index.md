---
title: "PSSaveAsPdf"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "Postscript を PDF に変換します"
type: docs
weight: 10
url: /ja/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Postscript を PDF に変換します。

```js
function AsposePSSaveAsPdf(
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`不明なエラーが発生しました: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
