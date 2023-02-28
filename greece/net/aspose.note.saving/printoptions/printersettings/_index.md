---
title: PrintOptions.PrinterSettings
second_title: Aspose.Note for .NET API Reference
description: PrintOptions ιδιοκτησία. Λαμβάνει ή ορίζει τις ρυθμίσεις του εκτυπωτή.
type: docs
weight: 40
url: /el/net/aspose.note.saving/printoptions/printersettings/
---
## PrintOptions.PrinterSettings property

Λαμβάνει ή ορίζει τις ρυθμίσεις του εκτυπωτή.

```csharp
public PrinterSettings PrinterSettings { get; set; }
```

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

* class [PrintOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../printoptions/)
* συνέλευση [Aspose.Note](../../../)


