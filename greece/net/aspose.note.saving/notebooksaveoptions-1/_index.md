---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions τάξη. Μια αφηρημένη βασική κλάση που αντιπροσωπεύει επιλογές αποθήκευσης σημειωματάριων για μια συγκεκριμένη μορφή και παρέχει κοινές επιλογές αποθήκευσης για όλους τους θυγατρικούς κόμβους εγγράφων.
type: docs
weight: 800
url: /el/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Μια αφηρημένη βασική κλάση που αντιπροσωπεύει επιλογές αποθήκευσης σημειωματάριων για μια συγκεκριμένη μορφή και παρέχει κοινές επιλογές αποθήκευσης για όλους τους θυγατρικούς κόμβους εγγράφων.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| TDocumentSaveOptions | Οι επιλογές αποθήκευσης για όλα τα θυγατρικά έγγραφα του notebook. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να αποθηκευτούν ρητά. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Λαμβάνει ή ορίζει τις επιλογές αποθήκευσης για όλα τα θυγατρικά έγγραφα του σημειωματάριου. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται ισοπεδωμένη. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Λαμβάνει τη μορφή με την οποία είναι αποθηκευμένο το σημειωματάριο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Λαμβάνει τις επιλογές αποθήκευσης για όλα τα θυγατρικά έγγραφα του notebook. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


