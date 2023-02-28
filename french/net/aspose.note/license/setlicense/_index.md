---
title: License.SetLicense
second_title: Référence de l'API Aspose.Note pour .NET
description: License méthode. Licence du composant.
type: docs
weight: 20
url: /fr/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licence du composant.

```csharp
public void SetLicense(string licenseName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| licenseName | String | Peut être un nom de fichier complet ou court ou le nom d'une ressource intégrée. Utilisez une chaîne vide pour passer en mode d'évaluation. |

### Remarques

Essaie de trouver la licence aux emplacements suivants :

1. Chemin explicite.

2. Le dossier qui contient l'assemblage du composant Aspose.

3. Le dossier qui contient l'assembly appelant du client.

4. Le dossier qui contient l'assembly d'entrée (démarrage).

5. Une ressource intégrée dans l'assembly appelant du client.

**Note:**Sur le .NET Compact Framework, essaie de trouver la licence uniquement dans ces emplacements :

1. Chemin explicite.

2. Une ressource intégrée dans l'assembly appelant du client.

### Exemples

Montre comment charger une licence pour Aspose.Note à partir d'un fichier.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Montre comment charger une licence pour Aspose.Note à partir d'une ressource de fichier intégrée.

```csharp
// Instanciation de la classe Licence
Aspose.Note.License license = new Aspose.Note.License();

// Passe uniquement le nom du fichier de licence intégré dans l'assembly
license.SetLicense("Aspose.Note.lic");
```

### Voir également

* class [License](../)
* espace de noms [Aspose.Note](../../license/)
* Assemblée [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Licence du composant.

```csharp
public void SetLicense(Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Un flux qui contient la licence. |

### Remarques

Utilisez cette méthode pour charger une licence à partir d'un flux.

### Exemples

Montre comment charger une licence pour Aspose.Note à partir d'un flux.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Voir également

* class [License](../)
* espace de noms [Aspose.Note](../../license/)
* Assemblée [Aspose.Note](../../../)


