---
title: "AsposePageAbout"
second_title: "Aspose.Page для JavaScript через C++"
description: "Получить информацию о продукте."
type: docs
url: /ru/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Получить информацию о продукте.

```js
function AsposePageAbout()
```

### Возвращаемое значение

Объект JSON
| Поле | Описание |
| ----- | ----------- |
| errorCode | код ошибки (0 нет ошибки) |
| errorText | текстовая ошибка ("" нет ошибки) |
| продукт | Название продукта |
| версия | Версия продукта |
| islicensed | Продукт лицензирован |


```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //PageAbout - Get info about Product
    const json = AsposePageModule.AsposePageAbout();
    console.log("PageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```
