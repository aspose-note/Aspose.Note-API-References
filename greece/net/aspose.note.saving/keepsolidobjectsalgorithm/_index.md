---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm τάξη. Μετακινεί το πλήρες αντικείμενο στην επόμενη σελίδα σε περίπτωση που δεν χωράει στην αρχική σελίδα.
type: docs
weight: 740
url: /el/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

Μετακινεί το πλήρες αντικείμενο στην επόμενη σελίδα σε περίπτωση που δεν χωράει στην αρχική σελίδα.

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`KeepSolidObjectsAlgorithm` κλάση που χρησιμοποιεί προεπιλεγμένο όριο ύψους κλωνοποιημένου τμήματος. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | Αρχικοποιεί μια νέα παρουσία του`KeepSolidObjectsAlgorithm` κλάση που χρησιμοποιεί συγκεκριμένο όριο ύψους κλωνοποιημένου τμήματος. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | Λαμβάνει το όριο ύψους του κλωνοποιημένου τμήματος. |

## Πεδία

| Ονομα | Περιγραφή |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | Το προεπιλεγμένο μέγιστο μέγεθος του κλωνοποιημένου τμήματος. |

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

Δείχνει τον τρόπο αποστολής εγγράφου σε εκτυπωτή χρησιμοποιώντας τυπικό παράθυρο διαλόγου των Windows με καθορισμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


