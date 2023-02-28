---
title: NoteTask.DueDate
second_title: Aspose.Note för .NET API-referens
description: NoteTask fast egendom. Hämtar eller ställer in förfallodatum.
type: docs
weight: 70
url: /sv/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

Hämtar eller ställer in förfallodatum.

```csharp
public DateTime DueDate { get; set; }
```

### Fastighetsvärde

DenDateTime .

### Exempel

Visar hur man genererar en pdf som innehåller alla sidor relaterade till 'Projekt A'.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Ladda dokumentet i Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

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

### Se även

* class [NoteTask](../)
* namnutrymme [Aspose.Note](../../notetask/)
* hopsättning [Aspose.Note](../../../)


