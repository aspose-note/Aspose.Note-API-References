---
title: MergeOptions.InsertAt
second_title: Aspose.Note voor .NET API-referentie
description: MergeOptions eigendom. Haalt of stelt de positie in waar geïmporteerde paginas worden ingevoegd.
type: docs
weight: 40
url: /nl/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

Haalt of stelt de positie in waar geïmporteerde pagina's worden ingevoegd.

```csharp
public int InsertAt { get; set; }
```

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException |  |

### Opmerkingen

Als de waarde groter is dan het aantal pagina's in het doeldocument, worden geïmporteerde pagina's toegevoegd aan het einde van het document.

### Voorbeelden

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

### Zie ook

* class [MergeOptions](../)
* naamruimte [Aspose.Note](../../mergeoptions/)
* montage [Aspose.Note](../../../)


