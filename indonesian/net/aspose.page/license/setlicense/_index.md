---
title: License.SetLicense
second_title: Aspose.Page untuk Referensi .NET API
description: License metode. Lisensi komponen.
type: docs
weight: 30
url: /id/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Lisensi komponen.

```csharp
public void SetLicense(string licenseName)
```

### Perkataan

Mencoba menemukan lisensi di lokasi berikut:

1. Jalur eksplisit.

2. Folder rakitan komponen.

3. Folder rakitan panggilan klien.

4. Folder rakitan entri.

5. Sumber daya tertanam dalam perakitan panggilan klien.

**Catatan:**Di .NET Compact Framework, mencoba menemukan lisensi hanya di lokasi berikut:

1. Jalur eksplisit.

2. Sumber daya tertanam dalam perakitan panggilan klien.

2. Folder file jar komponen.

### Contoh

Dalam contoh ini, upaya akan dilakukan untuk menemukan file lisensi bernama MyLicense.lic di folder yang berisi  komponen, di folder yang berisi rakitan pemanggil, di folder rakitan entri, lalu di sumber daya tertanam rakitan pemanggil.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

file jar komponen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Bisa berupa nama file lengkap atau pendek atau nama sumber daya tertanam. Gunakan string kosong untuk beralih ke mode evaluasi.

### Lihat juga

* class [License](../)
* ruang nama [Aspose.Page](../../license/)
* perakitan [Aspose.Page](../../../)

---

## SetLicense(Stream) {#setlicense}

Lisensi komponen.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Aliran yang berisi lisensi. |

### Perkataan

Gunakan metode ini untuk memuat lisensi dari aliran.

### Contoh

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### Lihat juga

* class [License](../)
* ruang nama [Aspose.Page](../../license/)
* perakitan [Aspose.Page](../../../)


