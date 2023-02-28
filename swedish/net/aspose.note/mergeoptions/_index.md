---
title: Class MergeOptions
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.MergeOptions klass. Alternativen för att slå samman en samling sidor.
type: docs
weight: 340
url: /sv/net/aspose.note/mergeoptions/
---
## MergeOptions class

Alternativen för att slå samman en samling sidor.

```csharp
public class MergeOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Hämtar eller ställer in ett värde som anger om tillhandahållna sidor ska importeras som enstaka sidor. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Hämtar eller ställer in ett värde som anger om infogade sidor ska läggas till som underordnade av föregående sida. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Hämtar eller ställer in positionen där importerade sidor ska infogas. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Hämtar eller ställer in avståndet mellan sidorna när de importeras som en enda sida. |

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

* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


