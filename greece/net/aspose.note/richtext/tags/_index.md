---
title: RichText.Tags
second_title: Aspose.Note for .NET API Reference
description: RichText ιδιοκτησία. Λαμβάνει τη λίστα με όλες τις ετικέτες μιας παραγράφου.
type: docs
weight: 90
url: /el/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Λαμβάνει τη λίστα με όλες τις ετικέτες μιας παραγράφου.

```csharp
public List<ITag> Tags { get; }
```

### Παραδείγματα

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

* interface [ITag](../../itag/)
* class [RichText](../)
* χώρος ονομάτων [Aspose.Note](../../richtext/)
* συνέλευση [Aspose.Note](../../../)


