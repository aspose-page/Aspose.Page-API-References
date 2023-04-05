---
title: License.SetLicense
second_title: Aspose.Page for .NET API Referansı
description: License yöntem. Bileşeni lisanslar.
type: docs
weight: 30
url: /tr/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Bileşeni lisanslar.

```csharp
public void SetLicense(string licenseName)
```

### Notlar

Lisansı aşağıdaki konumlarda bulmaya çalışır:

1. Açık yol.

2. Bileşen montajının klasörü.

3. İstemcinin çağrı derlemesinin klasörü.

4. Giriş düzeneğinin klasörü.

5. İstemcinin çağrı derlemesinde katıştırılmış bir kaynak.

**Not:**.NET Compact Framework üzerinde, lisansı yalnızca şu konumlarda bulmaya çalışır:

1. Açık yol.

2. İstemcinin çağrı derlemesinde katıştırılmış bir kaynak.

2. Bileşen jar dosyasının klasörü.

### Örnekler

Bu örnekte, içeren klasörde MyLicense.lic adlı bir lisans dosyası bulunmaya çalışılacaktır. bileşen, çağıran derlemeyi içeren klasörde, giriş derlemesinin klasöründe ve ardından çağıran derlemenin katıştırılmış kaynaklarında.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

bileşen jar dosyası:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Tam veya kısa bir dosya adı olabilir veya katıştırılmış bir kaynağın adı. Değerlendirme moduna geçmek için boş bir dize kullanın.

### Ayrıca bakınız

* class [License](../)
* ad alanı [Aspose.Page](../../license/)
* toplantı [Aspose.Page](../../../)

---

## SetLicense(Stream) {#setlicense}

Bileşeni lisanslar.

```csharp
public void SetLicense(Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Lisansı içeren bir akış. |

### Notlar

Akıştan lisans yüklemek için bu yöntemi kullanın.

### Örnekler

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

### Ayrıca bakınız

* class [License](../)
* ad alanı [Aspose.Page](../../license/)
* toplantı [Aspose.Page](../../../)


