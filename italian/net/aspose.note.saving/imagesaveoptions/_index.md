---
title: ImageSaveOptions
second_title: Aspose.Note per .NET API Reference
description: Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in immagini.
type: docs
weight: 700
url: /it/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in immagini.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions)(SaveFormat) | Inizializza una nuova istanza di[`ImageSaveOptions`](../imagesaveoptions) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions) { get; set; } | Ottiene o imposta le opzioni per la binarizzazione dell'immagine. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode) { get; set; } | Ottiene o imposta[`ColorMode`](./colormode) per l'immagine di output. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Ottiene o imposta le impostazioni del carattere da utilizzare durante il salvataggio |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Ottiene o imposta il numero di pagine da salvare. Per impostazione predefinita èMaxValue il che significa che tutte le pagine del documento verranno renderizzate. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Ottiene o imposta l'indice della prima pagina da salvare. Per impostazione predefinita è 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality) { get; set; } | Ottiene o imposta un valore che determina la qualità dell'immagine salvata. Questo valore viene passato al codec come parametro System.Drawing.Imaging.Encoder.Quality. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution) { get; set; } | Ottiene o imposta la risoluzione per le immagini generate, in punti per pollice. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Ottiene il formato in cui viene salvato il documento. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression) { get; set; } | Ottiene o imposta il tipo di compressione da utilizzare quando si salvano le immagini generate nel formato TIFF. |

### Esempi

Mostra come salvare un documento come immagine in formato Jpeg usando SaveFormat.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Salva il documento.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Mostra come impostare una qualità dell'immagine quando si salva un documento come immagine in formato JPEG.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Salva il documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Mostra come salvare un documento come immagine in formato Bmp utilizzando ImageSaveOptions.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Salva il documento.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Mostra come impostare una risoluzione dell'immagine durante il salvataggio del documento come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Salva il documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Mostra come salvare un documento come immagine in scala di grigi.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Salva il documento come gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Mostra come salvare un documento come immagine in formato Tiff usando la compressione PackBits.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Salva il documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Mostra come salvare il taccuino come immagine con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

Mostra come salvare un documento come immagine in formato Tiff usando la compressione Jpeg.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Salva il documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Mostra come salvare il taccuino appiattito come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

Mostra come salvare un documento come immagine in formato Tiff utilizzando la compressione fax CCITT Gruppo 3.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Salva il documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Mostra come salvare un documento in formato png.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Imposta l'indice della pagina
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Salva il documento come PNG.
oneFile.Save(dataDir, opts);
```

Mostra come salvare un documento come immagine binaria usando il metodo di Otsu.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Salva il documento come gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Mostra come salvare un documento come immagine binaria utilizzando una soglia fissa.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Salva il documento come gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### Guarda anche

* class [SaveOptions](../saveoptions)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
