---
title: "AsposePSMergeToPdf"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "Postscript ファイルを PDF に結合する"
type: docs
weight: 10
url: /ja/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Postscript ファイルを PDF に結合する。

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileNames | string | マージするファイルの名前。 |
| fileNameResult | string | 結果の PDF ファイル名。 |
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 関連項目

* function [PSSaveAsImage](../pssaveasimage/)
