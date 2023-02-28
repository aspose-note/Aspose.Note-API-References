---
title: Image.FileName
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Krijgt de bestandsnaam.
type: docs
weight: 60
url: /nl/net/aspose.note/image/filename/
---
## Image.FileName property

Krijgt de bestandsnaam.

```csharp
public string FileName { get; }
```

### Voorbeelden

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

* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


