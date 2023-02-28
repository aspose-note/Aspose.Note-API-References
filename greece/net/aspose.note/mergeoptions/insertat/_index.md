---
title: MergeOptions.InsertAt
second_title: Aspose.Note for .NET API Reference
description: MergeOptions ιδιοκτησία. Λαμβάνει ή ορίζει τη θέση όπου θα εισαχθούν οι εισαγόμενες σελίδες.
type: docs
weight: 40
url: /el/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

Λαμβάνει ή ορίζει τη θέση όπου θα εισαχθούν οι εισαγόμενες σελίδες.

```csharp
public int InsertAt { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException |  |

### Παρατηρήσεις

Εάν η τιμή είναι μεγαλύτερη από τον αριθμό των σελίδων στο έγγραφο προορισμού, τότε οι σελίδες εισαγωγής προστέθηκαν στο τέλος του εγγράφου.

### Παραδείγματα

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

### Δείτε επίσης

* class [MergeOptions](../)
* χώρος ονομάτων [Aspose.Note](../../mergeoptions/)
* συνέλευση [Aspose.Note](../../../)


