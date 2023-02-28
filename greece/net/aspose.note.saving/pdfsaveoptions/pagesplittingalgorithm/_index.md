---
title: PdfSaveOptions.PageSplittingAlgorithm
second_title: Aspose.Note for .NET API Reference
description: PdfSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει αλγόριθμο που χρησιμοποιείται για διαχωρισμό σελίδων.
type: docs
weight: 50
url: /el/net/aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/
---
## PdfSaveOptions.PageSplittingAlgorithm property

Λαμβάνει ή ορίζει αλγόριθμο που χρησιμοποιείται για διαχωρισμό σελίδων.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Αξία περιουσίας

Το`PageSplittingAlgorithm` .

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

Όταν οι μεγάλες σελίδες του OneNote αποθηκεύονται σε μορφή pdf, χωρίζονται σε σελίδες. Το δείγμα δείχνει πώς να διαμορφώσετε τη λογική διαχωρισμού των αντικειμένων που βρίσκονται στα διαλείμματα της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Όταν οι μεγάλες σελίδες του OneNote αποθηκεύονται σε μορφή pdf, χωρίζονται σε σελίδες. Το παράδειγμα δείχνει πώς να διαμορφώσετε τη λογική διαχωρισμού των αντικειμένων που βρίσκονται στα διαλείμματα της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Δείτε επίσης

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PdfSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../pdfsaveoptions/)
* συνέλευση [Aspose.Note](../../../)


