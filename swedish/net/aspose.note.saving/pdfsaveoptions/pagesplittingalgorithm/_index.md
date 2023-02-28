---
title: PdfSaveOptions.PageSplittingAlgorithm
second_title: Aspose.Note för .NET API-referens
description: PdfSaveOptions fast egendom. Hämtar eller ställer in algoritm som används för siddelning.
type: docs
weight: 50
url: /sv/net/aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/
---
## PdfSaveOptions.PageSplittingAlgorithm property

Hämtar eller ställer in algoritm som används för siddelning.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Fastighetsvärde

Den`PageSplittingAlgorithm` .

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

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PdfSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../pdfsaveoptions/)
* hopsättning [Aspose.Note](../../../)


