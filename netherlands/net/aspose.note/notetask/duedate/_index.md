---
title: NoteTask.DueDate
second_title: Aspose.Note voor .NET API-referentie
description: NoteTask eigendom. Haalt of stelt de vervaldatum in.
type: docs
weight: 70
url: /nl/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

Haalt of stelt de vervaldatum in.

```csharp
public DateTime DueDate { get; set; }
```

### Eigendoms-waarde

DeDateTime .

### Voorbeelden

Laat zien hoe je een pdf genereert met alle pagina's gerelateerd aan 'Project A'.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

* class [NoteTask](../)
* naamruimte [Aspose.Note](../../notetask/)
* montage [Aspose.Note](../../../)


