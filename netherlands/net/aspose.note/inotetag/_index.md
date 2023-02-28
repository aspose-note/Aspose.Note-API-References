---
title: Interface INoteTag
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.INoteTag koppel. De interface voor notitietags dwz tags die niet zijn gekoppeld aan Outlooktaken.
type: docs
weight: 180
url: /nl/net/aspose.note/inotetag/
---
## INoteTag interface

De interface voor notitietags (dwz tags die niet zijn gekoppeld aan Outlook-taken).

```csharp
public interface INoteTag : ITag
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Hiermee wordt de letterkleur opgehaald of ingesteld. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Haalt of stelt de markeringskleur in. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Haalt de labeltekst op of stelt deze in. |

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

* interface [ITag](../itag/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


