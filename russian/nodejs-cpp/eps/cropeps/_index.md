---
title: "AsposeCropEPS"
second_title: "Aspose.Page для JavaScript через C++"
description: "Обрезать EPS"
type: docs
weight: 10
url: /ru/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Обрезает файл EPS. Сохраняет исходный файл EPS с обновлённым существующим %%BoundingBox или создаёт новый.

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

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileBlob | Объект Blob | Содержимое исходного файла. |
| fileName | string | Имя исходного файла. |
| fileNameResult | string | Имя результирующего файла. |
| левый | float | Указывает левую границу области обрезки. |
| верхний | float | Указывает верхнюю границу области обрезки. |
| правый | float | Указывает правую границу области обрезки. |
| нижний | float | Указывает нижнюю границу области обрезки. |

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

### См. также

* function [AsposeResizeEps](../resizeeps/)
