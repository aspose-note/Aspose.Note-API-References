---
title: Document.Merge
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Voegt een reeks paginas samen in het document.
type: docs
weight: 120
url: /nl/net/aspose.note/document/merge/
---
## Document.Merge method

Voegt een reeks pagina's samen in het document.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pages | IEnumerable`1 | Een reeks pagina's. |
| mergeOptions | MergeOptions | Specificeert de opties voor het samenvoegen van aangeboden pagina's. |

### Winstwaarde

Retourneert de verwijzing naar het document.

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

### Zie ook

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


