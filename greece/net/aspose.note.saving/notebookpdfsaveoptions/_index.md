---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.NotebookPdfSaveOptions τάξη. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων σημειωματάριου σε PDF.
type: docs
weight: 780
url: /el/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων σημειωματάριου σε PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να αποθηκευτούν ρητά. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται ισοπεδωμένη. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


