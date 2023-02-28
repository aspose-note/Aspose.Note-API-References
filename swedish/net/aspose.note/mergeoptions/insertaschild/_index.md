---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note för .NET API-referens
description: MergeOptions fast egendom. Hämtar eller ställer in ett värde som anger om infogade sidor ska läggas till som underordnade av föregående sida.
type: docs
weight: 30
url: /sv/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Hämtar eller ställer in ett värde som anger om infogade sidor ska läggas till som underordnade av föregående sida.

```csharp
public bool InsertAsChild { get; set; }
```

### Exempel

Visar hur du importerar alla sidor från en uppsättning PDF-dokument samtidigt som du infogar sidor från varje PDF-dokument som underordnade OneNote-sidor.

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

### Se även

* class [MergeOptions](../)
* namnutrymme [Aspose.Note](../../mergeoptions/)
* hopsättning [Aspose.Note](../../../)


