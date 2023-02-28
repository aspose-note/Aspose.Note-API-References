---
title: Document.Merge
second_title: Aspose.Note per .NET API Reference
description: Document metodo. Unisce un insieme di pagine al documento.
type: docs
weight: 120
url: /it/net/aspose.note/document/merge/
---
## Document.Merge method

Unisce un insieme di pagine al documento.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pages | IEnumerable`1 | Un insieme di pagine. |
| mergeOptions | MergeOptions | Specifica le opzioni su come unire le pagine fornite. |

### Valore di ritorno

Restituisce il riferimento al documento.

### Esempi

Mostra come importare tutte le pagine dal documento PDF raggruppando ogni 5 pagine in una singola pagina di OneNote.

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

### Guarda anche

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)


