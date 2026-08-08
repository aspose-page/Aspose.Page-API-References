---
title: "AsposeResizeEPS"
second_title: "C++ 経由で JavaScript 用 Aspose.Page"
description: "EPS のリサイズ"
type: docs
weight: 10
url: /ja/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

EPS ファイルのサイズを変更します。既存の %%BoundingBox を更新した初期 EPS ファイルを保存するか、新しいものが作成されます。

```js
function AsposeResizeEPS(
    fileBlob,
    fileName, 
    fileNameResult, 
    width,
    height,
    units
)
```

| パラメーター | 型 | 説明 |
| --------- | ---- | ----------- |
| fileBlob | Blob オブジェクト | ソースファイルの内容。 |
| fileName | string | ソースファイル名。 |
| fileNameResult | string | 結果ファイル名。 |
| width | float | 新しいバウンディングボックスの幅を指定します。 |
| height | float | 新しいバウンディングボックスの高さを指定します。 |
| unit | Module.Units | 新しいサイズのタイプを指定します。 |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### 関連項目

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
