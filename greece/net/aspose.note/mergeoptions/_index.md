---
title: Class MergeOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.MergeOptions τάξη. Οι επιλογές για τη συγχώνευση συλλογής σελίδων.
type: docs
weight: 340
url: /el/net/aspose.note/mergeoptions/
---
## MergeOptions class

Οι επιλογές για τη συγχώνευση συλλογής σελίδων.

```csharp
public class MergeOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εισαχθούν παρεχόμενες σελίδες ως μία σελίδα. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι σελίδες που έχουν εισαχθεί πρέπει να προστεθούν ως θυγατρικές της προηγούμενης σελίδας. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Λαμβάνει ή ορίζει τη θέση όπου θα εισαχθούν οι εισαγόμενες σελίδες. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Λαμβάνει ή ορίζει το διάστημα μεταξύ των σελίδων όταν εισάγεται ως μία σελίδα. |

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

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


