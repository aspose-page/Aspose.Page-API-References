---
title: "AsposeEPSGetXmp"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Dapatkan metadata XMP"
type: docs
weight: 10
url: /id/nodejs-cpp/xmp/epsgetxmp/
---
## AsposeEPSGetXmp function

Membaca file PS/EPS dan mengekstrak XmpMetdata jika sudah ada.
Jika file EPS tidak mengandung metadata XMP, kami akan membuat yang baru yang diisi dengan nilai dari komentar metadata PS (%%Creator, %%CreateDate, %%Title, dll).
File EPS dengan metadata XMP yang terisi akan disimpan di fileNameResult.

```js
function AsposeEPSGetXmp(
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
|  | XMP | array nilai metadata |
|  | fileNameResult | nama file hasil |

### Contoh

```js
const AsposePage = require('asposepagenodejs');

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeEPSGetXMP(eps_file, img_file + "_out.eps");
    console.log("AsposeEPSGetXMP => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

* function [XPSSaveAsImage](../xpssaveasimage/)
