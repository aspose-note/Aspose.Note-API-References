---
title: Image.HorizontalOffset
second_title: Référence de l'API Aspose.Note pour .NET
description: Image propriété. Obtient ou définit le décalage horizontal.
type: docs
weight: 100
url: /fr/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

Obtient ou définit le décalage horizontal.

```csharp
public float HorizontalOffset { get; set; }
```

### Exemples

Montre comment ajouter une image d'un fichier à un document avec des propriétés définies par l'utilisateur.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document à partir du flux.
Document doc = new Document(dataDir + "Aspose.one");

// Récupère la première page du document.
Aspose.Note.Page page = doc.FirstChild;

// Charge une image à partir du fichier.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Modifiez la taille de l'image selon vos besoins (optionnel).
                              Width = 100,
                              Height = 100,

                              // Définit l'emplacement de l'image dans la page (optionnel).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Définir l'alignement de l'image
                              Alignment = HorizontalAlignment.Right
                          };

// Ajoute l'image à la page.
page.AppendChildLast(image);
```

### Voir également

* class [Image](../)
* espace de noms [Aspose.Note](../../image/)
* Assemblée [Aspose.Note](../../../)


