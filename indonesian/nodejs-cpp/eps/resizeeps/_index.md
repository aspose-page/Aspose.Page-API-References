---
title: "AsposeResizeEPS"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Ubah ukuran EPS"
type: docs
weight: 10
url: /id/nodejs-cpp/eps/resizeeps/
---
## AsposeResizeEPS function

Mengubah ukuran file EPS. Ini menyimpan file EPS awal dengan %%BoundingBox yang ada diperbarui atau membuat yang baru.

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

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileBlob | Objek Blob | Konten file sumber. |
| fileName | string | Nama file sumber. |
| fileNameResult | string | Nama file hasil. |
| lebar | float | Menentukan lebar kotak pembatas baru. |
| tinggi | float | Menentukan tinggi kotak pembatas baru. |
| satuan | Module.Units | Menentukan tipe ukuran baru. |

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

    //ResizeEPS - working with EPS
    const json = AsposePageModule.AsposeResizeEPS(eps_file, "resized.eps", 200, 100, AsposePageModule.Units.Points);
    console.log("ResizeEPS => %O",  json.errorCode == 0 ? JSON.parse(JSON.stringify(json).replace('"errorCode":0,"errorText":"",','')) : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

* function [Module.Units](../../enumerations/units/)
* function [AsposeCropEps](../cropeps/)
