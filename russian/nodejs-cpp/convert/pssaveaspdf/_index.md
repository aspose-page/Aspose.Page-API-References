---
title: "PSSaveAsPdf"
second_title: "Aspose.Page для JavaScript через C++"
description: "Преобразует Postscript в PDF"
type: docs
weight: 10
url: /ru/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Преобразует Postscript в PDF.

```js
function AsposePSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileBlob | Объект Blob | Содержимое исходного шрифта для преобразования. |
| fileName | string | Имя файла. |
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page для Node.js через C++ примеры.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Произошла неизвестная ошибка: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
