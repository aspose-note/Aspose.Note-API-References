---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note for .NET API Reference
description: MergeOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι σελίδες που έχουν εισαχθεί πρέπει να προστεθούν ως θυγατρικές της προηγούμενης σελίδας.
type: docs
weight: 30
url: /el/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι σελίδες που έχουν εισαχθεί πρέπει να προστεθούν ως θυγατρικές της προηγούμενης σελίδας.

```csharp
public bool InsertAsChild { get; set; }
```

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


