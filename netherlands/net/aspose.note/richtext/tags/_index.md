---
title: RichText.Tags
second_title: Aspose.Note voor .NET API-referentie
description: RichText eigendom. Krijgt de lijst met alle tags van een paragraaf.
type: docs
weight: 90
url: /nl/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Krijgt de lijst met alle tags van een paragraaf.

```csharp
public List<ITag> Tags { get; }
```

### Voorbeelden

Laat zien hoe u toegang krijgt tot de details van de taken van Outlook.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tasks();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle RichText-knooppunten op
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Doorloop elk knooppunt
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Eigenschappen ophalen
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Zie ook

* interface [ITag](../../itag/)
* class [RichText](../)
* naamruimte [Aspose.Note](../../richtext/)
* montage [Aspose.Note](../../../)


