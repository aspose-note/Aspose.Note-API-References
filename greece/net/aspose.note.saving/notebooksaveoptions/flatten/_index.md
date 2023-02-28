---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note for .NET API Reference
description: NotebookSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται ισοπεδωμένη.
type: docs
weight: 20
url: /el/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται ισοπεδωμένη.

```csharp
public bool Flatten { get; set; }
```

### Παραδείγματα

Δείχνει πώς μπορείτε να αποθηκεύσετε πεπλατυσμένο σημειωματάριο σε μορφή pdf.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Αποθηκεύστε το Σημειωματάριο
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Δείχνει πώς να αποθηκεύσετε το πεπλατυσμένο σημειωματάριο ως εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir, notebookSaveOptions);
```

### Δείτε επίσης

* class [NotebookSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../notebooksaveoptions/)
* συνέλευση [Aspose.Note](../../../)


