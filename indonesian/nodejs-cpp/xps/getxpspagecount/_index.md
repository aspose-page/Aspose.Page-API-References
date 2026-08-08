---
title: "AsposeGetXpsPageCount"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Dapatkan jumlah halaman dalam file XPS"
type: docs
weight: 10
url: /id/nodejs-cpp/xps/getxpspagecount/
---
## AsposeGetXpsPageCount function

Dapatkan jumlah halaman dalam dokumen xps.

```js
function AsposeGetXpsPageCount(
    fileBlob,
    fileName
)
```

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileBlob | Objek Blob | Konten file sumber. |
| fileName | string | Nama file sumber. |

### Nilai Kembalian

Objek JSON
| Bidang | Deskripsi |
| ----- | ----------- |
|  | errorCode | kesalahan kode (0 tidak ada kesalahan) |
|  | errorText | kesalahan teks ("" tidak ada kesalahan) |
|  | pageCount | jumlah halaman |

### Contoh

```js
const AsposePage = require('asposepagenodejs');

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    let json = AsposePageModule.AsposePageAbout();
    console.log("AsposePageAbout => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : "error:" + json.errorText);

    //AsposeGetXpsPageCount
    json = AsposePageModule.AsposeGetXpsPageCount(xps_file);
    console.log("AsposeGetXpsPageCount => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```


