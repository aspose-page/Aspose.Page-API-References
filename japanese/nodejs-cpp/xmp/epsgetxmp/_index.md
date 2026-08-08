---
title: "AsposeEPSGetXmp"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "XMP メタデータを取得する"
type: docs
weight: 10
url: /ja/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

PS/EPS ファイルを読み取り、既に存在する場合は XMP メタデータを抽出します。
EPS ファイルに XMP メタデータが含まれていない場合、PS メタデータコメント（%%Creator、%%CreateDate、%%Title など）から取得した値で埋められた新しいメタデータを生成します。
XMP メタデータが埋め込まれた EPS ファイルは fileNameResult に保存されます。

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileBlob | Blob オブジェクト | ソースファイルの内容。 |
| fileName | string | ソースファイル名。 |
| fileNameResult | string | 結果ファイル名。 |


### 戻り値

JSON オブジェクト
| フィールド | 説明 |
| ----- | ----------- |
|  | errorCode | コードエラー (0 エラーなし) |
|  | errorText | テキストエラー ("" エラーなし) |
|  | XMP | メタデータ値の配列 |
|  | fileNameResult | 結果ファイル名 |

### 例

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

### 関連項目

* function [XPSSaveAsImage](../xpssaveasimage/)
