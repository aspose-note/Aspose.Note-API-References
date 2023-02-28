---
title: NoteTask.DueDate
second_title: Aspose.Note für .NET-API-Referenz
description: NoteTask eigendom. Ruft das Fälligkeitsdatum ab oder legt es fest.
type: docs
weight: 70
url: /de/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

Ruft das Fälligkeitsdatum ab oder legt es fest.

```csharp
public DateTime DueDate { get; set; }
```

### Eigentumswert

DieDateTime .

### Beispiele

Zeigt, wie man ein PDF generiert, das alle Seiten enthält, die sich auf „Projekt A“ beziehen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
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

Zeigt, wie auf Details der Outlook-Aufgaben zugegriffen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tasks();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle RichText-Knoten abrufen
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Durch jeden Knoten iterieren
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Eigenschaften abrufen
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Siehe auch

* class [NoteTask](../)
* namensraum [Aspose.Note](../../notetask/)
* Montage [Aspose.Note](../../../)


