---
title: PrintOptions.DocumentName
second_title: Aspose.Note for .NET API Reference
description: PrintOptions ιδιοκτησία. Λαμβάνει ή ορίζει το όνομα του εγγράφου που θα εμφανίζεται για παράδειγμα σε ένα παράθυρο διαλόγου κατάστασης εκτύπωσης ή σε ουρά εκτυπωτή κατά την εκτύπωση του εγγράφου.
type: docs
weight: 20
url: /el/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Λαμβάνει ή ορίζει το όνομα του εγγράφου που θα εμφανίζεται (για παράδειγμα, σε ένα παράθυρο διαλόγου κατάστασης εκτύπωσης ή σε ουρά εκτυπωτή) κατά την εκτύπωση του εγγράφου.

```csharp
public string DocumentName { get; set; }
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


