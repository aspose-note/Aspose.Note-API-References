---
title: Document.Import
second_title: Aspose.Note för .NET API-referens
description: Document metod. Importerar en uppsättning sidor från medföljande PDFdokument.
type: docs
weight: 110
url: /sv/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Importerar en uppsättning sidor från medföljande PDF-dokument.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | En ström med PDF-dokument. |
| importOptions | PdfImportOptions | Anger alternativen för hur man importerar sidor från PDF-dokument. |
| mergeOptions | MergeOptions | Anger alternativen för hur man slår samman angivna sidor. |

### Returvärde

Returnerar referensen till dokumentet.

### Se även

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namnutrymme [Aspose.Note](../../document/)
* hopsättning [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Importerar en uppsättning sidor från medföljande PDF-dokument.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | String | En fil med PDF-dokument. |
| importOptions | PdfImportOptions | Anger alternativen för hur man importerar sidor från PDF-dokument. |
| mergeOptions | MergeOptions | Anger alternativen för hur man slår samman angivna sidor. |

### Returvärde

Returnerar referensen till dokumentet.

### Exempel

Visar hur man importerar alla sidor från en uppsättning PDF-dokument sida för sida.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namnutrymme [Aspose.Note](../../document/)
* hopsättning [Aspose.Note](../../../)


