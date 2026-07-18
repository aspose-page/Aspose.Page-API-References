---
title: "XPSSaveAsPdf"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Mengonversi XPS ke PDF"
type: docs
weight: 10
url: /id/nodejs-cpp/convert/xpssaveaspdf/
---
## PSSaveAsPdf function

Mengonversi XPS ke PDF.

```js
function AsposeXPSSaveAsPdf(
    fileBlob, 
    fileName, 
    supressErrors
)
```

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileBlob | Objek Blob | Konten font sumber untuk konversi. |
| fileName | string | Nama file. |
| supressErrors | bool | Menentukan apakah kesalahan harus ditekan atau tidak. |

### Nilai Kembalian

Objek JSON
| Bidang | Deskripsi |
| ----- | ----------- |
|  | errorCode | kesalahan kode (0 tidak ada kesalahan) |
|  | errorText | kesalahan teks ("" tidak ada kesalahan) |
|  | fileNameResult | nama file hasil |

### Contoh

```js
const AsposePage = require('asposepagenodejs');

const xps_file = "./data/example.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSSaveAsPdf(xps_file,true);
    console.log("XPSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

* function [XPSSaveAsImage](../xpssaveasimage/)
