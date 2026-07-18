---
title: "XPSSaveAsImage"
second_title: "Aspose.Page для JavaScript через C++"
description: "Преобразует XPS в изображение"
type: docs
weight: 10
url: /ru/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Преобразует Postscript в изображение.

```js
function AsposeXPSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileBlob | Объект Blob | Содержимое исходного шрифта для преобразования. |
| fileName | string | Имя файла. |
| imageFormat | ImageFormat | формат изображения для преобразования. |
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

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### См. также

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
