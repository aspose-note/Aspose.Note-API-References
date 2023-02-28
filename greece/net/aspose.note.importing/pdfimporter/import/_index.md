---
title: PdfImporter.Import
second_title: Aspose.Note for .NET API Reference
description: PdfImporter μέθοδος. Εισάγει περιεχόμενο του εγγράφου PDF από μια παρεχόμενη ροή.
type: docs
weight: 10
url: /el/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Εισάγει περιεχόμενο του εγγράφου PDF από μια παρεχόμενη ροή.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Η ροή. |
| options | PdfImportOptions | Οι επιλογές. |

### Επιστρεφόμενη Αξία

Το[`PdfImporter`](../) .

### Δείτε επίσης

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* χώρος ονομάτων [Aspose.Note.Importing](../../pdfimporter/)
* συνέλευση [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Εισάγει περιεχόμενο του εγγράφου PDF από ένα καθορισμένο αρχείο.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | String | Το αρχείο PDF. |
| options | PdfImportOptions | Οι επιλογές. |

### Επιστρεφόμενη Αξία

Το[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* χώρος ονομάτων [Aspose.Note.Importing](../../pdfimporter/)
* συνέλευση [Aspose.Note](../../../)


