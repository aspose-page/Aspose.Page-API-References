---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page для JavaScript через C++"
description: "Объединить файлы XPS в один XPS"
type: docs
weight: 10
url: /ru/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Объединить несколько файлов XPS в один файл XPS.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileNames | string | Имена файлов для объединения. |
| fileNameResult | string | Имя результирующего XPS-файла. |
| supressErrors | bool | Указывает, должны ли ошибки подавляться или нет. |

### Возвращаемое значение

Объект JSON
| Поле | Описание |
| ----- | ----------- |
|  | errorCode | код ошибки (0 нет ошибки) |
|  | errorText | текстовая ошибка ("" нет ошибки) |
|  | fileNameResult | имя результирующего файла |

### Примеры

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

### См. также

* function [XPSMergeToPdf](../xpsmergetopdf/)
