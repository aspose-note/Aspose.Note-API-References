---
title: Document.Import
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Εισάγει ένα σύνολο σελίδων από το παρεχόμενο έγγραφο PDF.
type: docs
weight: 110
url: /el/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Εισάγει ένα σύνολο σελίδων από το παρεχόμενο έγγραφο PDF.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Μια ροή με έγγραφο PDF. |
| importOptions | PdfImportOptions | Καθορίζει τις επιλογές για τον τρόπο εισαγωγής σελίδων από έγγραφο PDF. |
| mergeOptions | MergeOptions | Καθορίζει τις επιλογές για τη συγχώνευση παρεχόμενων σελίδων. |

### Επιστρεφόμενη Αξία

Επιστρέφει την αναφορά στο έγγραφο.

### Δείτε επίσης

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Εισάγει ένα σύνολο σελίδων από το παρεχόμενο έγγραφο PDF.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | String | Ένα αρχείο με έγγραφο PDF. |
| importOptions | PdfImportOptions | Καθορίζει τις επιλογές για τον τρόπο εισαγωγής σελίδων από έγγραφο PDF. |
| mergeOptions | MergeOptions | Καθορίζει τις επιλογές για τη συγχώνευση παρεχόμενων σελίδων. |

### Επιστρεφόμενη Αξία

Επιστρέφει την αναφορά στο έγγραφο.

### Παραδείγματα

Δείχνει τον τρόπο εισαγωγής όλων των σελίδων από ένα σύνολο εγγράφων PDF σελίδα προς σελίδα.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

Δείχνει πώς να εισάγετε όλες τις σελίδες από ένα σύνολο εγγράφων PDF, ενώ εισάγετε σελίδες από κάθε έγγραφο PDF ως παιδιά μιας σελίδας OneNote ανώτατου επιπέδου.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

Δείχνει πώς να εισάγετε όλο το περιεχόμενο από ένα σύνολο εγγράφων PDF ενώ συγχωνεύετε σελίδες από κάθε έγγραφο PDF σε μια μεμονωμένη σελίδα OneNote.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### Δείτε επίσης

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


