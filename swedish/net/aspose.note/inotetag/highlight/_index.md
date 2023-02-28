---
title: INoteTag.Highlight
second_title: Aspose.Note för .NET API-referens
description: INoteTag fast egendom. Hämtar eller ställer in högdagerfärgen.
type: docs
weight: 20
url: /sv/net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

Hämtar eller ställer in högdagerfärgen.

```csharp
public Color Highlight { get; set; }
```

### Exempel

Visar hur du kommer åt information om en tagg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Hämta alla RichText-noder
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterera genom varje nod
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Hämta egenskaper
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### Se även

* interface [INoteTag](../)
* namnutrymme [Aspose.Note](../../inotetag/)
* hopsättning [Aspose.Note](../../../)


