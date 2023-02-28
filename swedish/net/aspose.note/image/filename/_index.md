---
title: Image.FileName
second_title: Aspose.Note för .NET API-referens
description: Image fast egendom. Hämtar filnamnet.
type: docs
weight: 60
url: /sv/net/aspose.note/image/filename/
---
## Image.FileName property

Hämtar filnamnet.

```csharp
public string FileName { get; }
```

### Exempel

Visar hur man får bildens metainformation.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla bildnoder
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

### Se även

* class [Image](../)
* namnutrymme [Aspose.Note](../../image/)
* hopsättning [Aspose.Note](../../../)


