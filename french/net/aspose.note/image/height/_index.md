---
title: Image.Height
second_title: Référence de l'API Aspose.Note pour .NET
description: Image propriété. Obtient ou définit la hauteur. Il sagit de la hauteur réelle de limage dans le document MS OneNote.
type: docs
weight: 90
url: /fr/net/aspose.note/image/height/
---
## Image.Height property

Obtient ou définit la hauteur. Il s'agit de la hauteur réelle de l'image dans le document MS OneNote.

```csharp
public float Height { get; set; }
```

### Exemples

Montre comment obtenir les méta-informations de l'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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


