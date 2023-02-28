---
title: Image.FileName
second_title: Référence de l'API Aspose.Note pour .NET
description: Image propriété. Récupère le nom du fichier.
type: docs
weight: 60
url: /fr/net/aspose.note/image/filename/
---
## Image.FileName property

Récupère le nom du fichier.

```csharp
public string FileName { get; }
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

### Voir également

* class [Image](../)
* espace de noms [Aspose.Note](../../image/)
* Assemblée [Aspose.Note](../../../)


