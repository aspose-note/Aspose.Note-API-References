---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note voor .NET API-referentie
description: MergeOptions eigendom. Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of ingevoegde paginas moeten worden toegevoegd als onderliggende paginas van de vorige pagina.
type: docs
weight: 30
url: /nl/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of ingevoegde pagina's moeten worden toegevoegd als onderliggende pagina's van de vorige pagina.

```csharp
public bool InsertAsChild { get; set; }
```

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


