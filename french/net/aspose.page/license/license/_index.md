---
title: License.License
second_title: Aspose.Page pour la référence de l'API .NET
description: License constructeur. Initialise une nouvelle instance de cette classe.
type: docs
weight: 10
url: /fr/net/aspose.page/license/license/
---
## License constructor

Initialise une nouvelle instance de cette classe.

```csharp
public License()
```

### Exemples

Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic dans le dossier qui contient  le composant, dans le dossier qui contient l'assembly appelant, dans le dossier de l'assembly d'entrée puis dans les ressources embarquées de l'assembly appelant.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

le fichier jar du composant :

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Voir également

* class [License](../)
* espace de noms [Aspose.Page](../../license/)
* Assemblée [Aspose.Page](../../../)


