---
title: MergeOptions.ImportAsSinglePage
second_title: Aspose.Note voor .NET API-referentie
description: MergeOptions eigendom. Haalt een waarde op of stelt een waarde in die aangeeft of de aangeboden paginas als enkele pagina moeten worden geïmporteerd.
type: docs
weight: 20
url: /nl/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

Haalt een waarde op of stelt een waarde in die aangeeft of de aangeboden pagina's als enkele pagina moeten worden geïmporteerd.

```csharp
public bool ImportAsSinglePage { get; set; }
```

### Voorbeelden

Laat zien hoe u alle pagina's uit een PDF-document kunt importeren, waarbij u elke 5 pagina's naar één OneNote-pagina groepeert.

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

Laat zien hoe u alle inhoud van een set PDF-documenten importeert terwijl u pagina's van elk PDF-document samenvoegt tot één OneNote-pagina.

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

### Zie ook

* class [MergeOptions](../)
* naamruimte [Aspose.Note](../../mergeoptions/)
* montage [Aspose.Note](../../../)


