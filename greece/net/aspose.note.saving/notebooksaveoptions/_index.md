---
title: Class NotebookSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.NotebookSaveOptions τάξη. Μια αφηρημένη βασική κλάση που αντιπροσωπεύει επιλογές αποθήκευσης σημειωματάριων για μια συγκεκριμένη μορφή.
type: docs
weight: 790
url: /el/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

Μια αφηρημένη βασική κλάση που αντιπροσωπεύει επιλογές αποθήκευσης σημειωματάριων για μια συγκεκριμένη μορφή.

```csharp
public abstract class NotebookSaveOptions
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να αποθηκευτούν ρητά. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται ισοπεδωμένη. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Λαμβάνει τη μορφή με την οποία είναι αποθηκευμένο το σημειωματάριο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Λαμβάνει τις επιλογές αποθήκευσης για όλα τα θυγατρικά έγγραφα του notebook. |

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

* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


