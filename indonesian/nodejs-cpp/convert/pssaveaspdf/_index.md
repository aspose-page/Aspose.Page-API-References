---
title: "PSSaveAsPdf"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Mengonversi Postscript ke PDF"
type: docs
weight: 10
url: /id/nodejs-cpp/convert/pssaveaspdf/
---
## PSSaveAsPdf function

Mengonversi Postscript ke PDF.

```js
function AsposePSSaveAsPdf(
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
```js
const AsposePage = require('asposepagenodejs');

const ps_file = "./data/program_13.ps";

console.log("Aspose.Page untuk Node.js via contoh C++.");

AsposePage().then(AsposePageModule => {

const json = AsposePageModule.AsposePSSaveAsPdf(ps_file, true);
console.log("PSSaveAsPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
reason => {console.log(`Kesalahan tidak diketahui telah terjadi: ${reason}`);}
);
```

### See Also

* function [PSSaveAsImage](../pssaveasimage/)
