---
title: Class NotebookLoadOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.NotebookLoadOptions τάξη. Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός σημειωματάριου.
type: docs
weight: 420
url: /el/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός σημειωματάριου.

```csharp
public class NotebookLoadOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να φορτωθούν ρητά αργότερα. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να φορτωθούν κατά τη φόρτωση του γονικού εγγράφου. |

### Παραδείγματα

Δείχνει πώς να κάνετε ένα κρυπτογραφημένο σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


