---
title: CheckBox.SetOpen
second_title: Aspose.Note for .NET API Reference
description: CheckBox μέθοδος. Ορίζει την ετικέτα σε κατάσταση ανοίγματος.
type: docs
weight: 80
url: /el/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Ορίζει την ετικέτα σε κατάσταση ανοίγματος.

```csharp
public virtual void SetOpen()
```

### Παραδείγματα

Δείχνει πώς μπορείτε να ανοίξετε όλα τα στοιχεία του πλαισίου ελέγχου που σχετίζονται με το «Έργο Γ».

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

### Δείτε επίσης

* class [CheckBox](../)
* χώρος ονομάτων [Aspose.Note](../../checkbox/)
* συνέλευση [Aspose.Note](../../../)


