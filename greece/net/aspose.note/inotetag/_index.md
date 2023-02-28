---
title: Interface INoteTag
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.INoteTag διεπαφή. Η διεπαφή για ετικέτες σημειώσεων δηλαδή ετικέτες που δεν σχετίζονται με εργασίες του Outlook.
type: docs
weight: 180
url: /el/net/aspose.note/inotetag/
---
## INoteTag interface

Η διεπαφή για ετικέτες σημειώσεων (δηλαδή ετικέτες που δεν σχετίζονται με εργασίες του Outlook).

```csharp
public interface INoteTag : ITag
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Παίρνει ή ορίζει το χρώμα της γραμματοσειράς. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα επισήμανσης. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Λαμβάνει ή ορίζει το κείμενο της ετικέτας. |

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

* interface [ITag](../itag/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


