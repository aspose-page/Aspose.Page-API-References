---
title: License.License
second_title: Aspose.Page per riferimento all'API .NET
description: License costruttore. Inizializza una nuova istanza di questa classe.
type: docs
weight: 10
url: /it/net/aspose.page/license/license/
---
## License constructor

Inizializza una nuova istanza di questa classe.

```csharp
public License()
```

### Esempi

In questo esempio, verrà effettuato un tentativo di trovare un file di licenza denominato MyLicense.lic nella cartella che contiene  il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di entrata e poi nelle risorse embedded dell'assembly chiamante.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

il file jar del componente:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Guarda anche

* class [License](../)
* spazio dei nomi [Aspose.Page](../../license/)
* assemblea [Aspose.Page](../../../)


