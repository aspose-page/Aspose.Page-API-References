---
title: "AsposePSMergeToPdf"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Gabungkan file Postscript ke PDF"
type: docs
weight: 10
url: /id/nodejs-cpp/merge/psmergetopdf/
---
## AsposePSMergeToPdf function

Gabungkan file Postscript ke PDF.

```js
function AsposePSMergePdf(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileNames | string | Nama-nama file untuk digabungkan. |
| fileNameResult | string | Nama file pdf hasil. |
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

const ps_files = "./data/program_01.ps,./data/PAGENET-361-10.eps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposePSMergeToPdf(ps_files,"PsMergedToPdfResult.pdf",true);
    console.log("PSMergeToPdf => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);
},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

* function [PSSaveAsImage](../pssaveasimage/)
