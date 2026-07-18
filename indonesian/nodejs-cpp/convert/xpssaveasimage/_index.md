---
title: "XPSSaveAsImage"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Mengonversi XPS ke gambar"
type: docs
weight: 10
url: /id/nodejs-cpp/convert/xpssaveasimage/
---
## PSSaveAsImage function

Mengonversi Postscript ke gambar.

```js
function AsposeXPSSaveAsImage(
    fileBlob, 
    fileName, 
    imageFormat, 
    supressErrors
)
```

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileBlob | Objek Blob | Konten font sumber untuk konversi. |
| fileName | string | Nama file. |
| imageFormat | ImageFormat | format gambar untuk dikonversi menjadi. |
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

    const json = AsposePageModule.AsposeXPSSaveAsImage(xps_file,AsposePageModule.ImageFormat.Png,true);
    console.log("XPSSaveAsImage => %O",  json.errorCode == 0 ? "Files(pages) count: " + json.filesCount.toString() + json.filesNameResult.toString() : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

* function [XPSSaveAsPdf](../xpssaveaspdf/)
* enum [ImageFormat](../../enumerations/imageformat/)
