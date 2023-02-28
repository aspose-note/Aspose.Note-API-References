---
title: Class PdfSaveOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.PdfSaveOptions classe. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in PDF.
type: docs
weight: 850
url: /it/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Ottiene o imposta le impostazioni del carattere da utilizzare durante il salvataggio |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | Ottiene o imposta il tipo di compressione applicato alle immagini nel file PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | Ottiene o imposta un valore che determina la qualità delle immagini JPEG all'interno del documento PDF. Il valore può variare da 0 a 100 dove 0 indica la qualità peggiore ma la compressione massima e 100 indica la qualità migliore ma la compressione minima. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. Per impostazione predefinita èMaxValue che significa che verranno visualizzate tutte le pagine del documento. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice della prima pagina da salvare. Di default è 0. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | Ottiene o imposta le impostazioni di pagina per ogni pagina nel documento. Per impostazione predefinita dipende da CurrentUICulture, *le culture statunitensi hanno l'impostazione lettera, altre hanno impostazioni A4. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | Ottiene o imposta l'algoritmo utilizzato per la suddivisione della pagina. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Ottiene il formato in cui viene salvato il documento. |

### Esempi

Mostra come salvare un documento in formato Pdf con layout di pagina Lettera.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Salva il documento.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Mostra come salvare un documento in formato Pdf con layout di pagina A4 senza limiti di altezza.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Salva il documento.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Mostra come salvare il notebook in formato pdf con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

Quando le pagine lunghe di OneNote vengono salvate in formato pdf, vengono suddivise tra le pagine. L'esempio mostra come configurare la logica di suddivisione degli oggetti posizionati sulle interruzioni di pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Mostra come salvare un documento in formato pdf.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Imposta l'indice della prima pagina da salvare
                              PageIndex = 0,

                              // Imposta il conteggio delle pagine
                              PageCount = 1,
                          };

// Salva il documento come PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Mostra come salvare un documento in formato pdf utilizzando impostazioni specifiche.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Usa la compressione Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualità per la compressione JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Quando le pagine lunghe di OneNote vengono salvate in formato pdf, vengono suddivise tra le pagine. L'esempio mostra come configurare la logica di suddivisione degli oggetti posti sulle interruzioni di pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Guarda anche

* class [SaveOptions](../saveoptions/)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


