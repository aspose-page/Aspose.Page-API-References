---
title: "AsposeSaveImageAsEps"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Ubah ukuran EPS"
type: docs
weight: 10
url: /id/nodejs-cpp/image/saveimageaseps/
---
## AsposeSaveImageAsEps function

Mengubah ukuran file EPS. Ini menyimpan file EPS awal dengan %%BoundingBox yang ada diperbarui atau membuat yang baru.

```js
function AsposeSaveImageAsEps(
    fileBlob,
    fileName, 
    fileNameResult
)
```

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileBlob | Objek Blob | Konten file sumber. |
| fileName | string | Nama file sumber. |
| fileNameResult | string | Nama file hasil. |

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

const img_file = "./data/PAGENET-361-10.bmp";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    //SaveImageAsEps - convert image to EPS
    const json = AsposePageModule.AsposeSaveImageAsEps(img_file, img_file + ".eps");
    console.log("SaveImageAsEps => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

