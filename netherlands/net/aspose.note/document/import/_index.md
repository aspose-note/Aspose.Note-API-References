---
title: Document.Import
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Importeert een set paginas uit het meegeleverde PDFdocument.
type: docs
weight: 110
url: /nl/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Importeert een set pagina's uit het meegeleverde PDF-document.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | Een stream met PDF-document. |
| importOptions | PdfImportOptions | Specificeert de opties voor het importeren van pagina's uit een PDF-document. |
| mergeOptions | MergeOptions | Specificeert de opties voor het samenvoegen van aangeboden pagina's. |

### Winstwaarde

Retourneert de verwijzing naar het document.

### Zie ook

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Importeert een set pagina's uit het meegeleverde PDF-document.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| file | String | Een bestand met PDF-document. |
| importOptions | PdfImportOptions | Specificeert de opties voor het importeren van pagina's uit een PDF-document. |
| mergeOptions | MergeOptions | Specificeert de opties voor het samenvoegen van aangeboden pagina's. |

### Winstwaarde

Retourneert de verwijzing naar het document.

### Voorbeelden

Laat zien hoe u pagina voor pagina alle pagina's uit een set PDF-documenten importeert.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


