---
title: Class ImageSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.ImageSaveOptions klas. Maakt het mogelijk om extra opties te specificeren bij het renderen van documentpaginas naar afbeeldingen.
type: docs
weight: 720
url: /nl/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Maakt het mogelijk om extra opties te specificeren bij het renderen van documentpagina's naar afbeeldingen.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Initialiseert een nieuw exemplaar van het`ImageSaveOptions` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Krijgt of stelt opties in voor de binarisatie van afbeeldingen. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Krijgt of zet[`ColorMode`](./colormode/) voor de uitvoerafbeelding. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Haalt lettertype-instellingen op of stelt deze in om te gebruiken tijdens het opslaan |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Haalt het aantal op te slaan pagina's op of stelt het in. Standaard isMaxValue wat betekent dat alle pagina's van het document worden weergegeven. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Haalt of stelt de index in van de eerste pagina die moet worden opgeslagen. Standaard is 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die de kwaliteit van de opgeslagen afbeelding bepaalt. Deze waarde wordt doorgegeven aan de codec als System.Drawing.Imaging.Encoder.Quality-parameter. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Hiermee wordt de resolutie voor de gegenereerde afbeeldingen opgehaald of ingesteld, in dots per inch. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Haalt de indeling op waarin het document is opgeslagen. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Hiermee wordt het type compressie opgehaald of ingesteld dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |

### Voorbeelden

Laat zien hoe u een document kunt opslaan als afbeelding in JPEG-indeling met behulp van SaveFormat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Sla het document op.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Laat zien hoe u een afbeeldingskwaliteit instelt wanneer u een document opslaat als afbeelding in JPEG-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Sla het document op.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Laat zien hoe u een document kunt opslaan als afbeelding in Bmp-indeling met behulp van ImageSaveOptions.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Sla het document op.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Laat zien hoe u een afbeeldingsresolutie instelt bij het opslaan van een document als afbeelding.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Sla het document op.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Laat zien hoe u een document opslaat als afbeelding in grijstinten.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Sla het document op als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Laat zien hoe u een document opslaat als afbeelding in Tiff-indeling met behulp van PackBits-compressie.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Sla het document op.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Laat zien hoe u een notitieblok kunt opslaan als afbeelding met opgegeven opties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

Laat zien hoe u een document kunt opslaan als afbeelding in Tiff-indeling met behulp van JPEG-compressie.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Sla het document op.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Laat zien hoe u een afgeplat notitieboek als afbeelding kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

Laat zien hoe u een document kunt opslaan als afbeelding in Tiff-indeling met behulp van CCITT Groep 3-faxcompressie.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Sla het document op.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Laat zien hoe u een document opslaat in png-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialiseer het ImageSaveOptions-object 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Stel pagina-index in
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Sla het document op als PNG.
oneFile.Save(dataDir, opts);
```

Laat zien hoe u een document opslaat als binaire afbeelding met behulp van de methode van Otsu.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Sla het document op als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Laat zien hoe u een document opslaat als binaire afbeelding met een vaste drempel.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Sla het document op als gif.
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

### Zie ook

* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


