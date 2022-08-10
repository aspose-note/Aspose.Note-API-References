---
title: PdfSaveOptions
second_title: Aspose.Note för .NET API-referens
description: Gör det möjligt att ange ytterligare alternativ när du renderar dokumentsidor till PDF.
type: docs
weight: 820
url: /sv/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Gör det möjligt att ange ytterligare alternativ när du renderar dokumentsidor till PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Hämtar eller ställer in teckensnittets inställningar som ska användas medan de sparas |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | Hämtar eller ställer in typen av komprimering som tillämpas på bilder i PDF-filen. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | Hämtar eller ställer in ett värde som bestämmer kvaliteten på JPEG-bilderna i PDF-dokumentet. Värdet kan variera från 0 till 100 där 0 betyder sämsta kvalitet men maximal komprimering och 100 betyder bästa kvalitet men minsta komprimering. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Hämtar eller ställer in antalet sidor som ska sparas. Som standard ärMaxValue vilket innebär att alla sidor i dokumentet kommer att renderas. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Hämtar eller ställer in indexet för den första sidan som ska sparas. Som standard är 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | Hämtar eller ställer in algoritm som används för siddelning. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Hämtar formatet som dokumentet sparas i. |

### Exempel

Visar hur du sparar anteckningsboken i pdf-format med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

När långa OneNote-sidor sparas i pdf-format delas de upp på sidor. Exemplet visar hur man konfigurerar uppdelningslogiken för objekt som finns på sidavbrott.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Visar hur man sparar ett dokument i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ställ in sidindex för första sidan som ska sparas
                              PageIndex = 0,

                              // Ställ in sidantal
                              PageCount = 1,
                          };

// Spara dokumentet som PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Visar hur man sparar ett dokument i pdf-format med specifika inställningar.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Använd Jpeg-komprimering
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kvalitet för JPEG-komprimering
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

När långa OneNote-sidor sparas i pdf-format delas de upp på sidor. Exemplet visar hur man konfigurerar uppdelningslogiken för objekt som finns på sidavbrott.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Eller
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
