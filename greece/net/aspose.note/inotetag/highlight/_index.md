---
title: INoteTag.Highlight
second_title: Aspose.Note for .NET API Reference
description: INoteTag ιδιοκτησία. Λαμβάνει ή ορίζει το χρώμα επισήμανσης.
type: docs
weight: 20
url: /el/net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

Λαμβάνει ή ορίζει το χρώμα επισήμανσης.

```csharp
public Color Highlight { get; set; }
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


