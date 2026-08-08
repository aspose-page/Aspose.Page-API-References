---
title: "AsposeCropEPS"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "EPS をトリミング"
type: docs
weight: 10
url: /ja/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

EPS ファイルをトリミングします。既存の %%BoundingBox を更新した初期 EPS ファイルを保存するか、新しいファイルが作成されます。

```js
function AsposeCropEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    left,
    top,
    right,
    bottom
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileBlob | Blob オブジェクト | ソースファイルの内容。 |
| fileName | string | ソースファイル名。 |
| fileNameResult | string | 結果ファイル名。 |
| 左 | float | トリミングボックスの左境界を指定します。 |
| 上 | float | トリミングボックスの上境界を指定します。 |
| 右 | float | トリミングボックスの右境界を指定します。 |
| 下 | float | トリミングボックスの下境界を指定します。 |

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

const eps_file = "./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //CropEPS - working with EPS
    const json = AsposePageModule.AsposeCropEPS(eps_file, "croped.eps", 30, 5, 240, 36);
    console.log("CropEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 関連項目

* function [AsposeResizeEps](../resizeeps/)
