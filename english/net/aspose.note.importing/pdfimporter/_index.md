---
title: Class PdfImporter
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Importing.PdfImporter class. The class providing api to import content from documents in PDF format. The api allows to import from PDF document located either in a file or in a stream using specified options. The import options are passed using PdfImportOptions
type: docs
weight: 290
url: /net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

The class providing api to import content from documents in PDF format. The api allows to import from PDF document located either in a file or in a stream using specified options. The import options are passed using [`PdfImportOptions`](../pdfimportoptions/).

```csharp
public static class PdfImporter
```

## Methods

| Name | Description |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Imports content of PDF document from a provided stream. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Imports content of PDF document from a specified file. |

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

* namespace [Aspose.Note.Importing](../../aspose.note.importing/)
* assembly [Aspose.Note](../../)


