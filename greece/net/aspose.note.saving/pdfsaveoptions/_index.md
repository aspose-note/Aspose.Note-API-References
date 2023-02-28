---
title: Class PdfSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.PdfSaveOptions τάξη. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων εγγράφου σε PDF.
type: docs
weight: 850
url: /el/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων εγγράφου σε PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις της γραμματοσειράς που θα χρησιμοποιηθούν κατά την αποθήκευση |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο συμπίεσης που εφαρμόζεται σε εικόνες στο αρχείο PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. Η τιμή μπορεί να ποικίλλει από 0 έως 100 όπου 0 σημαίνει χειρότερη ποιότητα αλλά μέγιστη συμπίεση και 100 σημαίνει καλύτερη ποιότητα αλλά ελάχιστη συμπίεση. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων προς αποθήκευση. Από προεπιλογή είναιMaxValue που σημαίνει ότι όλες οι σελίδες του εγγράφου θα αποδοθούν. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας προς αποθήκευση. Από προεπιλογή είναι 0. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. Από προεπιλογή εξαρτάται από το CurrentUICulture, *Οι πολιτισμοί των ΗΠΑ έχουν ρύθμιση γραμμάτων, ενώ άλλοι έχουν ρυθμίσεις A4. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | Λαμβάνει ή ορίζει αλγόριθμο που χρησιμοποιείται για διαχωρισμό σελίδων. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Λαμβάνει τη μορφή στην οποία είναι αποθηκευμένο το έγγραφο. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή Pdf με διάταξη σελίδας Letter.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή Pdf με διάταξη σελίδας Α4 χωρίς όριο ύψους.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
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

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Αρχικοποίηση αντικειμένου PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ορισμός ευρετηρίου σελίδας της πρώτης σελίδας που θα αποθηκευτεί
                              PageIndex = 0,

                              // Ορισμός αριθμού σελίδων
                              PageCount = 1,
                          };

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας συγκεκριμένες ρυθμίσεις.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Αρχικοποίηση αντικειμένου PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Χρησιμοποιήστε συμπίεση Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Ποιότητα για συμπίεση JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


