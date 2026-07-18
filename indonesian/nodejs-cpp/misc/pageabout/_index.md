---
title: "AsposePageAbout"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Dapatkan info tentang Produk."
type: docs
url: /id/nodejs-cpp/misc/asposepageabout/
---

## AsposeFontAbout function

Dapatkan info tentang Produk.

```js
function AsposePageAbout()
```

### Nilai kembali

Objek JSON
| Bidang | Deskripsi |
| ----- | ----------- |
| errorCode | kesalahan kode (0 tidak ada kesalahan) |
| errorText | kesalahan teks ("" tidak ada kesalahan) |
| produk | Nama produk |
| versi | Versi produk |
| islicensed | Produk berlisensi |


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
