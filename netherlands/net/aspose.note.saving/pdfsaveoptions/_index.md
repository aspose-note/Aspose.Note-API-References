---
title: Class PdfSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.PdfSaveOptions klas. Maakt het mogelijk om extra opties te specificeren bij het renderen van documentpaginas naar PDF.
type: docs
weight: 850
url: /nl/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Maakt het mogelijk om extra opties te specificeren bij het renderen van documentpagina's naar PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Haalt lettertype-instellingen op of stelt deze in om te gebruiken tijdens het opslaan |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | Hiermee wordt het type compressie dat wordt toegepast op afbeeldingen in het PDF-bestand opgehaald of ingesteld. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die de kwaliteit van de JPEG-afbeeldingen in een PDF-document bepaalt. De waarde kan variëren van 0 tot 100, waarbij 0 de slechtste kwaliteit maar maximale compressie betekent en 100 de beste kwaliteit maar minimale compressie betekent. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Haalt het aantal op te slaan pagina's op of stelt het in. Standaard isMaxValue wat betekent dat alle pagina's van het document worden weergegeven. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Haalt of stelt de index in van de eerste pagina die moet worden opgeslagen. Standaard is 0. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | Hiermee worden de pagina-instellingen voor elke pagina in het document opgehaald of ingesteld. Standaard afhankelijk van CurrentUICulture, *Amerikaanse culturen hebben letterinstellingen, andere hebben A4-instellingen. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | Haalt of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Haalt de indeling op waarin het document is opgeslagen. |

### Voorbeelden

Laat zien hoe u een document in pdf-indeling kunt opslaan met de pagina-indeling Letter.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Sla het document op.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Laat zien hoe u een document opslaat in Pdf-formaat met A4-paginalay-out zonder hoogtebeperking.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Sla het document op.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Laat zien hoe u een notitieblok in pdf-indeling kunt opslaan met opgegeven opties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

Wanneer lange OneNote-pagina's in pdf-indeling worden opgeslagen, worden ze over pagina's verdeeld. Het voorbeeld laat zien hoe u de splitsingslogica configureert van objecten die zich op pagina-einden bevinden.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// of
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Laat zien hoe u een document opslaat in pdf-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Stel de pagina-index in van de eerste pagina die moet worden opgeslagen
                              PageIndex = 0,

                              // Stel het aantal pagina's in
                              PageCount = 1,
                          };

// Sla het document op als PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Laat zien hoe u een document in pdf-formaat kunt opslaan met behulp van specifieke instellingen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Gebruik JPEG-compressie
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kwaliteit voor JPEG-compressie
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Wanneer lange OneNote-pagina's in pdf-indeling worden opgeslagen, worden ze over pagina's verdeeld. Het voorbeeld laat zien hoe u de splitsingslogica configureert van objecten die zich op pagina-einden bevinden.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Of
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Zie ook

* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


