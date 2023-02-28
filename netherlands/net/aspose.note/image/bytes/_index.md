---
title: Image.Bytes
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Haalt de afbeeldingsgegevensopslag op.
type: docs
weight: 50
url: /nl/net/aspose.note/image/bytes/
---
## Image.Bytes property

Haalt de afbeeldingsgegevensopslag op.

```csharp
public byte[] Bytes { get; }
```

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

### Zie ook

* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


