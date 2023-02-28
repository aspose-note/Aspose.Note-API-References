---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm τάξη. Προσθέτει το επάνω μέρος του αντικειμένου στο κάτω μέρος της σελίδας και κλωνοποιεί το πλήρες αντικείμενο στην επόμενη σελίδα σε περίπτωση που δεν χωράει στην αρχική σελίδα.
type: docs
weight: 730
url: /el/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Προσθέτει το επάνω μέρος του αντικειμένου στο κάτω μέρος της σελίδας και κλωνοποιεί το πλήρες αντικείμενο στην επόμενη σελίδα σε περίπτωση που δεν χωράει στην αρχική σελίδα.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`KeepPartAndCloneSolidObjectToNextPageAlgorithm` κλάση, χρησιμοποιώντας προεπιλεγμένο όριο ύψους κλωνοποιημένου τμήματος. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Αρχικοποιεί μια νέα παρουσία του`KeepPartAndCloneSolidObjectToNextPageAlgorithm` κλάση, χρησιμοποιώντας συγκεκριμένο όριο ύψους κλωνοποιημένου τμήματος. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Λαμβάνει το όριο ύψους του κλωνοποιημένου τμήματος. |

## Πεδία

| Ονομα | Περιγραφή |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | Το προεπιλεγμένο μέγιστο μέγεθος του κλωνοποιημένου τμήματος. |

### Παραδείγματα

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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


