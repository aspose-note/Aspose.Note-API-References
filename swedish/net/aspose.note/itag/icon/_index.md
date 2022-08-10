---
title: Icon
second_title: Aspose.Note för .NET API-referens
description: Hämtar eller ställer in ikonen.
type: docs
weight: 30
url: /sv/net/aspose.note/itag/icon/
---
## ITag.Icon property

Hämtar eller ställer in ikonen.

```csharp
public TagIcon Icon { get; }
```

### Fastighetsvärde

Den[`TagIcon`](../../tagicon) .

### Exempel

Visar hur du kommer åt detaljer om Outlooks uppgifter.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tasks();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla RichText-noder
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterera genom varje nod
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Hämta egenskaper
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

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

* enum [TagIcon](../../tagicon)
* interface [ITag](../../itag)
* namnutrymme [Aspose.Note](../../itag)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->