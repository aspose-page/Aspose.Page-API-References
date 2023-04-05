---
title: License.SetLicense
second_title: Aspose.Page voor .NET API-referentie
description: License methode. Licentie voor de component.
type: docs
weight: 30
url: /nl/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licentie voor de component.

```csharp
public void SetLicense(string licenseName)
```

### Opmerkingen

Probeert de licentie te vinden op de volgende locaties:

1. Expliciet pad.

2. De map van de componentassemblage.

3. De map van de aanroepende assembly van de client.

4. De map van de ingangsassemblage.

5. Een ingesloten bron in de aanroepende assembly van de client.

**Opmerking:**Probeert op het .NET Compact Framework de licentie alleen op deze locaties te vinden:

1. Expliciet pad.

2. Een ingesloten bron in de aanroepende assembly van de client.

2. De map van het jar-bestand van de component.

### Voorbeelden

In dit voorbeeld wordt geprobeerd een licentiebestand met de naam MyLicense.lic te vinden in de map die bevat de component, in de map die de aanroepende assembly bevat, in de map van de entry-assembly en vervolgens in de ingebedde bronnen van de aanroepende assembly.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

het component jar-bestand:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Kan een volledige of korte bestandsnaam zijn of de naam van een ingesloten bron. Gebruik een lege string om over te schakelen naar de evaluatiemodus.

### Zie ook

* class [License](../)
* naamruimte [Aspose.Page](../../license/)
* montage [Aspose.Page](../../../)

---

## SetLicense(Stream) {#setlicense}

Licentie voor de component.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | Een stream die de licentie bevat. |

### Opmerkingen

Gebruik deze methode om een licentie van een stream te laden.

### Voorbeelden

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

### Zie ook

* class [License](../)
* naamruimte [Aspose.Page](../../license/)
* montage [Aspose.Page](../../../)


