---
title: Document.Merge
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Συγχωνεύει ένα σύνολο σελίδων στο έγγραφο.
type: docs
weight: 120
url: /el/net/aspose.note/document/merge/
---
## Document.Merge method

Συγχωνεύει ένα σύνολο σελίδων στο έγγραφο.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pages | IEnumerable`1 | Ένα σύνολο σελίδων. |
| mergeOptions | MergeOptions | Καθορίζει τις επιλογές για τη συγχώνευση παρεχόμενων σελίδων. |

### Επιστρεφόμενη Αξία

Επιστρέφει την αναφορά στο έγγραφο.

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

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


