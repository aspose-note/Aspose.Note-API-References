---
title: Document.Merge
second_title: Aspose.Note for .NET API Reference
description: Document method. Merges a set of pages to the document
type: docs
weight: 120
url: /net/aspose.note/document/merge/
---
## Document.Merge method

Merges a set of pages to the document.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pages | IEnumerable`1 | A set of pages. |
| mergeOptions | MergeOptions | Specifies the options how to merge provided pages. |

### Return Value

Returns the reference to the document.

## Examples

Shows how to import all pages from PDF document grouping every 5 pages to a single OneNote page.

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

### See Also

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


