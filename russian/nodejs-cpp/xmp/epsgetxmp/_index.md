---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page для JavaScript через C++"
description: "Получить XMP‑метаданные"
type: docs
weight: 10
url: /ru/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Читает файл PS/EPS и извлекает XMP‑метаданные, если они уже существуют.
Если EPS‑файл не содержит XMP‑метаданных, мы получаем новые, заполненные значениями из комментариев метаданных PS (%%Creator, %%CreateDate, %%Title и т.д.).
EPS‑файл с заполненными XMP‑метаданными будет сохранён в fileNameResult.

```js
function AsposeEPSGetXmp(
    fileBlob, 
    fileName, 
    fileNameResult
)
```

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileBlob | Объект Blob | Содержимое исходного файла. |
| fileName | string | Имя исходного файла. |
| fileNameResult | string | Имя результирующего файла. |


### Возвращаемое значение

Объект JSON
| Поле | Описание |
| ----- | ----------- |
|  | errorCode | код ошибки (0 нет ошибки) |
|  | errorText | текстовая ошибка ("" нет ошибки) |
|  | XMP | массив значений метаданных |
|  | fileNameResult | имя результирующего файла |

### Примеры

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

### См. также

* function [XPSSaveAsImage](../xpssaveasimage/)
