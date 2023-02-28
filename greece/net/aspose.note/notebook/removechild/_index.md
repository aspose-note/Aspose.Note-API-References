---
title: Notebook.RemoveChild
second_title: Aspose.Note for .NET API Reference
description: Notebook μέθοδος. Αφαιρεί τον θυγατρικό κόμβο.
type: docs
weight: 140
url: /el/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

Αφαιρεί τον θυγατρικό κόμβο.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldChild | INotebookChildNode | Ο κόμβος προς κατάργηση. |

### Επιστρεφόμενη Αξία

Ο κόμβος που αφαιρέθηκε.

### Παραδείγματα

Δείχνει τον τρόπο πρόσβασης σε όλες τις ενότητες από ένα σημειωματάριο.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
```

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

Δείχνει πώς να αποθηκεύσετε ένα σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### Δείτε επίσης

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* χώρος ονομάτων [Aspose.Note](../../notebook/)
* συνέλευση [Aspose.Note](../../../)


