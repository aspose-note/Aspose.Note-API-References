---
title: PageSettings.Letter
second_title: Aspose.Note for .NET API Reference
description: PageSettings ιδιοκτησία. Λαμβάνει ρυθμίσεις για τη σελίδα Letterformat.
type: docs
weight: 30
url: /el/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Λαμβάνει ρυθμίσεις για τη σελίδα Letter-format.

```csharp
public static PageSettings Letter { get; }
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

### Δείτε επίσης

* class [PageSettings](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../pagesettings/)
* συνέλευση [Aspose.Note](../../../)


