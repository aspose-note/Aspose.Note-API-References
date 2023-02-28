---
title: NoteTask.DueDate
second_title: Aspose.Note for .NET API Reference
description: NoteTask ιδιοκτησία. Λαμβάνει ή ορίζει την ημερομηνία λήξης.
type: docs
weight: 70
url: /el/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

Λαμβάνει ή ορίζει την ημερομηνία λήξης.

```csharp
public DateTime DueDate { get; set; }
```

### Αξία περιουσίας

ΤοDateTime .

### Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα pdf που περιέχει όλες τις σελίδες που σχετίζονται με το 'Project A'.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

Δείχνει τον τρόπο πρόσβασης σε λεπτομέρειες των εργασιών του Outlook.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tasks();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Επανάληψη σε κάθε κόμβο
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Ανάκτηση ιδιοτήτων
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Δείτε επίσης

* class [NoteTask](../)
* χώρος ονομάτων [Aspose.Note](../../notetask/)
* συνέλευση [Aspose.Note](../../../)


