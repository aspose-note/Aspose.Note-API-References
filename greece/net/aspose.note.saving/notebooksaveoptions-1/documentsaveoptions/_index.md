---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note for .NET API Reference
description: NotebookSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει τις επιλογές αποθήκευσης για όλα τα θυγατρικά έγγραφα του σημειωματάριου.
type: docs
weight: 10
url: /el/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Λαμβάνει ή ορίζει τις επιλογές αποθήκευσης για όλα τα θυγατρικά έγγραφα του σημειωματάριου.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το σημειωματάριο σε μορφή pdf με καθορισμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir, notebookSaveOptions);
```

### Δείτε επίσης

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* συνέλευση [Aspose.Note](../../../)


