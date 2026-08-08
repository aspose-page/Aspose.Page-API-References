---
title: "AsposeXPSMergeToXps"
second_title: "Aspose.Page untuk JavaScript via C++"
description: "Gabungkan file XPS menjadi satu XPS"
type: docs
weight: 10
url: /id/nodejs-cpp/merge/xpsmergetoxps/
---
## AsposeXPSMergeToXps function

Gabungkan beberapa file XPS menjadi satu file XPS.

```js
function AsposeXPSMergeXps(
    fileNames, 
    fileNameResult, 
    supressErrors
)
```

| Parameter | Tipe | Deskripsi |
| --------- | ---- | ----------- |
| fileNames | string | Nama-nama file untuk digabungkan. |
| fileNameResult | string | Nama file xps hasil. |
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

const xps_files = "./data/example.xps,./data/transforms.xps";

console.log("Aspose.Page for Node.js via C++ examples.");

AsposePage().then(AsposePageModule => {

    const json = AsposePageModule.AsposeXPSMergeToXps(xps_files,"XpsMergedToXpsResult.xps");
    console.log("XPSMergeToXps => %O",  json.errorCode == 0 ? json.fileNameResult : json.errorText);

},
    reason => {console.log(`The unknown error has occurred: ${reason}`);}
);
```

### Lihat Juga

* function [XPSMergeToPdf](../xpsmergetopdf/)
