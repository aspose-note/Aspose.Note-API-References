---
title: PdfImporter.Import
second_title: Aspose.Note voor .NET API-referentie
description: PdfImporter methode. Importeert inhoud van PDFdocument uit een geleverde stream.
type: docs
weight: 10
url: /nl/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Importeert inhoud van PDF-document uit een geleverde stream.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom. |
| options | PdfImportOptions | De opties. |

### Winstwaarde

De[`PdfImporter`](../) .

### Zie ook

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* naamruimte [Aspose.Note.Importing](../../pdfimporter/)
* montage [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Importeert inhoud van PDF-document uit een opgegeven bestand.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| file | String | Het PDF-bestand. |
| options | PdfImportOptions | De opties. |

### Winstwaarde

De[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* naamruimte [Aspose.Note.Importing](../../pdfimporter/)
* montage [Aspose.Note](../../../)


