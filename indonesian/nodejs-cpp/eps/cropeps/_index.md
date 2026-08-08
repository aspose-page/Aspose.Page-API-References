---
title: "AsposeCropEPS"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Potong EPS"
type: docs
weight: 10
url: /id/nodejs-cpp/eps/cropeps/
---
## AsposeCropEPS function

Memotong file EPS. Ini menyimpan file EPS awal dengan %%BoundingBox yang ada diperbarui atau yang baru akan dibuat.

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

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileBlob | Objek Blob | Konten file sumber. |
| fileName | string | Nama file sumber. |
| fileNameResult | string | Nama file hasil. |
| kiri | float | Menentukan batas kiri kotak pemotongan. |
| atas | float | Menentukan batas atas kotak pemotongan. |
| kanan | float | Menentukan batas kanan kotak pemotongan. |
| bawah | float | Menentukan batas bawah kotak pemotongan. |

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

### Lihat Juga

* function [AsposeResizeEps](../resizeeps/)
