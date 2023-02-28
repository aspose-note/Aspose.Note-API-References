---
title: CompositeNode1.GetChildNodes
second_title: Référence de l'API Aspose.Note pour .NET
description: CompositeNode méthode. Obtenir tous les nœuds enfants par le type de nœud.
type: docs
weight: 70
url: /fr/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Obtenir tous les nœuds enfants par le type de nœud.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Paramètre | La description |
| --- | --- |
| T1 | Type d'éléments dans la liste renvoyée. |

### Return_Value

Une liste de nœuds enfants.

### Exemples

Montre comment obtenir une image à partir d'un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Images();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds Image
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Enregistre les octets de l'image dans un fichier
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* espace de noms [Aspose.Note](../../compositenode-1/)
* Assemblée [Aspose.Note](../../../)


