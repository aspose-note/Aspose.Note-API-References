---
title: Class PrintOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.PrintOptions τάξη. Επιλογές που χρησιμοποιούνται για την εκτύπωση ενός εγγράφου.
type: docs
weight: 860
url: /el/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Επιλογές που χρησιμοποιούνται για την εκτύπωση ενός εγγράφου.

```csharp
public class PrintOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [PrintOptions](printoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Λαμβάνει ή ορίζει το όνομα του εγγράφου που θα εμφανίζεται (για παράδειγμα, σε ένα παράθυρο διαλόγου κατάστασης εκτύπωσης ή σε ουρά εκτυπωτή) κατά την εκτύπωση του εγγράφου. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Λαμβάνει ή ορίζει αλγόριθμο που χρησιμοποιείται για διαχωρισμό σελίδων. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις του εκτυπωτή. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Λαμβάνει ή ορίζει την ανάλυση για τις εικόνες που δημιουργούνται, σε κουκκίδες ανά ίντσα. |

### Παραδείγματα

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

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


