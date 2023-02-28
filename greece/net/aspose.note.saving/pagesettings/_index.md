---
title: Class PageSettings
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.PageSettings τάξη. Αντιπροσωπεύει τις ρυθμίσεις διάταξης για μια σελίδα.
type: docs
weight: 820
url: /el/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Αντιπροσωπεύει τις ρυθμίσεις διάταξης για μια σελίδα.

```csharp
public class PageSettings
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Λαμβάνει ρυθμίσεις για τη σελίδα σε μορφή A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Λαμβάνει ρυθμίσεις για τη σελίδα σε μορφή A4 με απεριόριστο ύψος. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Λαμβάνει ρυθμίσεις για τη σελίδα Letter-format. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Λαμβάνει ρυθμίσεις για τη σελίδα με μορφή Letter με απεριόριστο ύψος. |

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

* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


