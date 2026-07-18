---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page для JavaScript через C++"
description: "Объединить файлы Postscript в PDF"
type: docs
weight: 10
url: /ru/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Объединить файлы Postscript в PDF.

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileNames | string | Имена файлов для объединения. |
| fileNameResult | string | Имя результирующего PDF-файла. |
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### См. также

* function [PSSaveAsImage](../pssaveasimage/)
