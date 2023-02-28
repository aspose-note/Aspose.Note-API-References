---
title: Class PdfImporter
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Importing.PdfImporter classe. La classe che fornisce lAPI per importare contenuto da documenti in formato PDF. LAPI consente di importare da un documento PDF situato in un file o in un flusso utilizzando le opzioni specificate. Le opzioni di importazione vengono passate utilizzandoPdfImportOptions .
type: docs
weight: 270
url: /it/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

La classe che fornisce l'API per importare contenuto da documenti in formato PDF. L'API consente di importare da un documento PDF situato in un file o in un flusso utilizzando le opzioni specificate. Le opzioni di importazione vengono passate utilizzando[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Importa il contenuto del documento PDF da un flusso fornito. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Importa il contenuto del documento PDF da un file specificato. |

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

* spazio dei nomi [Aspose.Note.Importing](../../aspose.note.importing/)
* assemblea [Aspose.Note](../../)


