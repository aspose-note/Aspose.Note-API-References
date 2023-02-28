---
title: Class MergeOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.MergeOptions klas. De opties voor het samenvoegen van een verzameling paginas.
type: docs
weight: 340
url: /nl/net/aspose.note/mergeoptions/
---
## MergeOptions class

De opties voor het samenvoegen van een verzameling pagina's.

```csharp
public class MergeOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [MergeOptions](mergeoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Haalt een waarde op of stelt een waarde in die aangeeft of de aangeboden pagina's als enkele pagina moeten worden geïmporteerd. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of ingevoegde pagina's moeten worden toegevoegd als onderliggende pagina's van de vorige pagina. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Haalt of stelt de positie in waar geïmporteerde pagina's worden ingevoegd. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Hiermee wordt de afstand tussen pagina's opgehaald of ingesteld wanneer deze als een enkele pagina wordt geïmporteerd. |

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

Laat zien hoe u alle pagina's uit een set PDF-documenten importeert terwijl u pagina's uit elk PDF-document invoegt als onderliggende pagina's van een OneNote-pagina op het hoogste niveau.

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

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


