---
title: "AsposeXPSMergeToXps"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "XPS ファイルを 1つの XPS に結合する"
type: docs
weight: 10
url: /ja/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

複数の XPS ファイルを 1つの XPS ファイルに結合する。

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileNames | string | マージするファイルの名前。 |
| fileNameResult | string | 結果の XPS ファイル名。 |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 関連項目

* function [XPSMergeToPdf](../xpsmergetopdf/)
