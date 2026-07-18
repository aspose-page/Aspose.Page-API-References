---
title: "AsposeResizeEPS"
second_title: "Aspose.Page для JavaScript через C++"
description: "Изменить размер EPS"
type: docs
weight: 10
url: /ru/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Изменяет размер EPS‑файла. Сохраняет исходный EPS‑файл с обновлённым существующим %%BoundingBox или создаёт новый.

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

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileBlob | Объект Blob | Содержимое исходного файла. |
| fileName | string | Имя исходного файла. |
| fileNameResult | string | Имя результирующего файла. |
| width | float | Указывает ширину новой ограничивающей рамки. |
| height | float | Указывает высоту новой ограничивающей рамки. |
| unit | Module.Units | Указывает тип нового размера. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### См. также

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
