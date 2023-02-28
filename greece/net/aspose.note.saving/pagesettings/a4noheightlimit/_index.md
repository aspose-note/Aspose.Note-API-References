---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note for .NET API Reference
description: PageSettings ιδιοκτησία. Λαμβάνει ρυθμίσεις για τη σελίδα σε μορφή A4 με απεριόριστο ύψος.
type: docs
weight: 20
url: /el/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Λαμβάνει ρυθμίσεις για τη σελίδα σε μορφή A4 με απεριόριστο ύψος.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Παραδείγματα

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

* class [PageSettings](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../pagesettings/)
* συνέλευση [Aspose.Note](../../../)


