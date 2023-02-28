---
title: Class PdfImporter
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Importing.PdfImporter klas. De klasse die een api levert om inhoud uit documenten in PDFindeling te importeren. De api maakt het mogelijk om vanuit een PDFdocument in een bestand of in een stream te importeren met behulp van gespecificeerde opties. De importopties worden doorgegeven met behulp vanPdfImportOptions .
type: docs
weight: 270
url: /nl/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

De klasse die een api levert om inhoud uit documenten in PDF-indeling te importeren. De api maakt het mogelijk om vanuit een PDF-document in een bestand of in een stream te importeren met behulp van gespecificeerde opties. De importopties worden doorgegeven met behulp van[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Importeert inhoud van PDF-document uit een geleverde stream. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Importeert inhoud van PDF-document uit een opgegeven bestand. |

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

* naamruimte [Aspose.Note.Importing](../../aspose.note.importing/)
* montage [Aspose.Note](../../)


