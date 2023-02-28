---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm klass. Flyttar hela objektet till nästa sida om det inte får plats på originalsidan.
type: docs
weight: 740
url: /sv/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

Flyttar hela objektet till nästa sida om det inte får plats på originalsidan.

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | Initierar en ny instans av`KeepSolidObjectsAlgorithm` klass med standardhöjdgräns för klonad del. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | Initierar en ny instans av`KeepSolidObjectsAlgorithm` klass med specifik höjdgräns för klonad del. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | Hämtar höjdgränsen för den klonade delen. |

## Fält

| namn | Beskrivning |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | Standardmaxstorleken för den klonade delen. |

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

Visar hur man skickar dokument till en skrivare med standard Windows-dialogruta med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


