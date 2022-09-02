---
title: SetLicense
second_title: Aspose.Page per riferimento all'API .NET
description: concede in licenza il componente.
type: docs
weight: 30
url: /it/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

concede in licenza il componente.

```csharp
public void SetLicense(string licenseName)
```

### Osservazioni

Cerca di trovare la licenza nelle seguenti posizioni:

1. Percorso esplicito.

2. La cartella dell'assieme del componente.

3. La cartella dell'assembly chiamante del client.

4. La cartella dell'assembly di ingresso.

5. Una risorsa incorporata nell'assembly chiamante del client.

**Nota:**In .NET Compact Framework, prova a trovare la licenza solo in queste posizioni:

1. Percorso esplicito.

2. Una risorsa incorporata nell'assembly chiamante del client.

2. La cartella del file jar del componente.

### Esempi

In questo esempio, verrà effettuato un tentativo di trovare un file di licenza denominato MyLicense.lic nella cartella che contiene  il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di ingresso e quindi nelle risorse incorporate dell'assembly chiamante.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

il file jar del componente:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

Può essere un nome di file completo o breve o il nome di una risorsa incorporata. Utilizzare una stringa vuota per passare alla modalità di valutazione.

### Guarda anche

* class [License](../../license)
* spazio dei nomi [Aspose.Page](../../license)
* assemblea [Aspose.Page](../../../)

---

## SetLicense(Stream) {#setlicense}

concede in licenza il componente.

```csharp
public void SetLicense(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Un flusso che contiene la licenza. |

### Osservazioni

Utilizzare questo metodo per caricare una licenza da uno stream.

### Esempi

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

### Guarda anche

* class [License](../../license)
* spazio dei nomi [Aspose.Page](../../license)
* assemblea [Aspose.Page](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->