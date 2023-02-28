---
title: PdfImporter.Import
second_title: Aspose.Note per .NET API Reference
description: PdfImporter metodo. Importa il contenuto del documento PDF da un flusso fornito.
type: docs
weight: 10
url: /it/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Importa il contenuto del documento PDF da un flusso fornito.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso. |
| options | PdfImportOptions | Le opzioni. |

### Valore di ritorno

Il[`PdfImporter`](../) .

### Guarda anche

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* spazio dei nomi [Aspose.Note.Importing](../../pdfimporter/)
* assemblea [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Importa il contenuto del documento PDF da un file specificato.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | String | Il file PDF. |
| options | PdfImportOptions | Le opzioni. |

### Valore di ritorno

Il[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* spazio dei nomi [Aspose.Note.Importing](../../pdfimporter/)
* assemblea [Aspose.Note](../../../)


