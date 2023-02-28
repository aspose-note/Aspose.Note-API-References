---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note for .NET API Reference
description: PdfSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. Από προεπιλογή εξαρτάται από το CurrentUICulture Οι πολιτισμοί των ΗΠΑ έχουν ρύθμιση γραμμάτων ενώ άλλοι έχουν ρυθμίσεις A4.
type: docs
weight: 40
url: /el/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. Από προεπιλογή εξαρτάται από το CurrentUICulture, *Οι πολιτισμοί των ΗΠΑ έχουν ρύθμιση γραμμάτων, ενώ άλλοι έχουν ρυθμίσεις A4.

```csharp
public PageSettings PageSettings { get; set; }
```

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

### Δείτε επίσης

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../pdfsaveoptions/)
* συνέλευση [Aspose.Note](../../../)


