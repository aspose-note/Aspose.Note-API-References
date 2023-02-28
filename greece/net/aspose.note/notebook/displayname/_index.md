---
title: Notebook.DisplayName
second_title: Aspose.Note for .NET API Reference
description: Notebook ιδιοκτησία. Λαμβάνει ή ορίζει το εμφανιζόμενο όνομα.
type: docs
weight: 40
url: /el/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Λαμβάνει ή ορίζει το εμφανιζόμενο όνομα.

```csharp
public string DisplayName { get; set; }
```

### Παραδείγματα

Δείχνει πώς να αφαιρέσετε μια ενότητα από ένα σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Διασχίστε τους θυγατρικούς κόμβους του για αναζήτηση του επιθυμητού θυγατρικού στοιχείου
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Αφαιρέστε το Θυγατρικό Στοιχείο από το Σημειωματάριο
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir);
```

### Δείτε επίσης

* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)


