---
title: INoteTag.FontColor
second_title: Aspose.Note voor .NET API-referentie
description: INoteTag eigendom. Hiermee wordt de letterkleur opgehaald of ingesteld.
type: docs
weight: 10
url: /nl/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

Hiermee wordt de letterkleur opgehaald of ingesteld.

```csharp
public Color FontColor { get; set; }
```

### Voorbeelden

Laat zien hoe u toegang krijgt tot de details van een tag.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Haal alle RichText-knooppunten op
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Doorloop elk knooppunt
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Eigenschappen ophalen
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

### Zie ook

* interface [INoteTag](../)
* naamruimte [Aspose.Note](../../inotetag/)
* montage [Aspose.Note](../../../)


