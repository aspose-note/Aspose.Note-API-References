---
title: MergeOptions.PageSpacing
second_title: Aspose.Note för .NET API-referens
description: MergeOptions fast egendom. Hämtar eller ställer in avståndet mellan sidorna när de importeras som en enda sida.
type: docs
weight: 50
url: /sv/net/aspose.note/mergeoptions/pagespacing/
---
## MergeOptions.PageSpacing property

Hämtar eller ställer in avståndet mellan sidorna när de importeras som en enda sida.

```csharp
public float PageSpacing { get; set; }
```

### Exempel

Visar hur man importerar alla sidor från PDF-dokumentgruppering var 5:e sida till en enda OneNote-sida.

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

Visar hur du importerar allt innehåll från en uppsättning PDF-dokument samtidigt som du slår samman sidor från varje PDF-dokument till en enda OneNote-sida.

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

### Se även

* class [MergeOptions](../)
* namnutrymme [Aspose.Note](../../mergeoptions/)
* hopsättning [Aspose.Note](../../../)


