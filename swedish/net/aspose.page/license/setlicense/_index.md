---
title: License.SetLicense
second_title: Aspose.Page för .NET API-referens
description: License metod. Licensierar komponenten.
type: docs
weight: 30
url: /sv/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licensierar komponenten.

```csharp
public void SetLicense(string licenseName)
```

### Anmärkningar

Försöker hitta licensen på följande platser:

1. Explicit väg.

2. Mappen för komponentsammansättningen.

3. Mappen för klientens anropssammansättning.

4. Mappen för ingångssammansättningen.

5. En inbäddad resurs i klientens anropssammansättning.

**Notera:**På .NET Compact Framework försöker du hitta licensen endast på dessa platser:

1. Explicit väg.

2. En inbäddad resurs i klientens anropssammansättning.

2. Mappen för komponentjar-filen.

### Exempel

I det här exemplet kommer ett försök att göras att hitta en licensfil med namnet MyLicense.lic i mappen som innehåller  komponenten, i mappen som innehåller den anropande sammansättningen, i mappen för postsammansättningen och sedan i de inbäddade resurserna för den anropande sammansättningen.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

komponentjarfilen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Kan vara ett fullständigt eller kort filnamn eller namnet på en inbäddad resurs. Använd en tom sträng för att växla till utvärderingsläge.

### Se även

* class [License](../)
* namnutrymme [Aspose.Page](../../license/)
* hopsättning [Aspose.Page](../../../)

---

## SetLicense(Stream) {#setlicense}

Licensierar komponenten.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | En stream som innehåller licensen. |

### Anmärkningar

Använd den här metoden för att ladda en licens från en stream.

### Exempel

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

### Se även

* class [License](../)
* namnutrymme [Aspose.Page](../../license/)
* hopsättning [Aspose.Page](../../../)


