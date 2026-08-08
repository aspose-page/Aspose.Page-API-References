---
title: "AsposePageAbout"
second_title: "Aspose.Page para JavaScript vía C++"
description: "Obtener información sobre el Producto."
type: docs
url: /es/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Obtener información sobre el Producto.

```js
function AsposePageAbout()
```

### Valor de retorno

Objeto JSON
| Campo | Descripción |
| ----- | ----------- |
| errorCode | error de código (0 sin error) |
| errorText | error de texto ("" sin error) |
| producto | Nombre del producto |
| versión | Versión del producto |
| islicensed | El producto está licenciado |


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
