---
title: Class PdfImporter
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Importing.PdfImporter τάξη. Η κλάση που παρέχει api για εισαγωγή περιεχομένου από έγγραφα σε μορφή PDF. Το api επιτρέπει την εισαγωγή από έγγραφο PDF που βρίσκεται είτε σε αρχείο είτε σε ροή χρησιμοποιώντας καθορισμένες επιλογές. Οι επιλογές εισαγωγής περνούν χρησιμοποιώνταςPdfImportOptions .
type: docs
weight: 270
url: /el/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

Η κλάση που παρέχει api για εισαγωγή περιεχομένου από έγγραφα σε μορφή PDF. Το api επιτρέπει την εισαγωγή από έγγραφο PDF που βρίσκεται είτε σε αρχείο είτε σε ροή χρησιμοποιώντας καθορισμένες επιλογές. Οι επιλογές εισαγωγής περνούν χρησιμοποιώντας[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Εισάγει περιεχόμενο του εγγράφου PDF από μια παρεχόμενη ροή. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Εισάγει περιεχόμενο του εγγράφου PDF από ένα καθορισμένο αρχείο. |

### Παραδείγματα

Δείχνει τον τρόπο εισαγωγής όλων των σελίδων από την ομαδοποίηση εγγράφων PDF κάθε 5 σελίδες σε μία σελίδα OneNote.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note.Importing](../../aspose.note.importing/)
* συνέλευση [Aspose.Note](../../)


