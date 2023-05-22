---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note for .NET API Reference
description: MergeOptions property. Gets or sets a value indicating whether inserted pages should be added as a children of previous page
type: docs
weight: 30
url: /net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Gets or sets a value indicating whether inserted pages should be added as a children of previous page.

```csharp
public bool InsertAsChild { get; set; }
```

## Examples

Shows how to import all pages from a set of PDF documents while inserting pages from every PDF document as children of a top level OneNote page.

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

### See Also

* class [MergeOptions](../)
* namespace [Aspose.Note](../../mergeoptions/)
* assembly [Aspose.Note](../../../)


