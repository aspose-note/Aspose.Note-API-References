---
title: Document.Print
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.
type: docs
weight: 130
url: /el/net/aspose.note/document/print/
---
## Print() {#print}

Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.

```csharp
public void Print()
```

### Παραδείγματα

Δείχνει τον τρόπο αποστολής εγγράφου σε εκτυπωτή χρησιμοποιώντας τυπικό παράθυρο διαλόγου των Windows με προεπιλεγμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.

```csharp
public void Print(PrintOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | PrintOptions | Επιλογές που χρησιμοποιούνται για την εκτύπωση ενός εγγράφου. Μπορεί να είναι null. |

### Δείτε επίσης

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


