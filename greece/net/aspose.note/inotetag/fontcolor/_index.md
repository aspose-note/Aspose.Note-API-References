---
title: INoteTag.FontColor
second_title: Aspose.Note for .NET API Reference
description: INoteTag ιδιοκτησία. Παίρνει ή ορίζει το χρώμα της γραμματοσειράς.
type: docs
weight: 10
url: /el/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

Παίρνει ή ορίζει το χρώμα της γραμματοσειράς.

```csharp
public Color FontColor { get; set; }
```

### Παραδείγματα

Δείχνει τον τρόπο πρόσβασης σε λεπτομέρειες μιας ετικέτας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Λήψη όλων των κόμβων RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Επανάληψη σε κάθε κόμβο
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Ανάκτηση ιδιοτήτων
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

### Δείτε επίσης

* interface [INoteTag](../)
* χώρος ονομάτων [Aspose.Note](../../inotetag/)
* συνέλευση [Aspose.Note](../../../)


