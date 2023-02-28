---
title: MergeOptions.ImportAsSinglePage
second_title: Aspose.Note for .NET API Reference
description: MergeOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εισαχθούν παρεχόμενες σελίδες ως μία σελίδα.
type: docs
weight: 20
url: /el/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εισαχθούν παρεχόμενες σελίδες ως μία σελίδα.

```csharp
public bool ImportAsSinglePage { get; set; }
```

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

* class [MergeOptions](../)
* χώρος ονομάτων [Aspose.Note](../../mergeoptions/)
* συνέλευση [Aspose.Note](../../../)


