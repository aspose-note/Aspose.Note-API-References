---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note voor .NET API-referentie
description: CompositeNode methode. Alle onderliggende knooppunten ophalen op basis van het knooppunttype.
type: docs
weight: 70
url: /nl/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Alle onderliggende knooppunten ophalen op basis van het knooppunttype.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Beschrijving |
| --- | --- |
| T1 | Het type elementen in de geretourneerde lijst. |

### Winstwaarde

Een lijst met onderliggende knooppunten.

### Voorbeelden

Laat zien hoe u een afbeelding uit een document haalt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Bewaar afbeeldingsbytes in een bestand
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Laat zien hoe u de meta-informatie van de afbeelding kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
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

### Zie ook

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* naamruimte [Aspose.Note](../../compositenode-1/)
* montage [Aspose.Note](../../../)


