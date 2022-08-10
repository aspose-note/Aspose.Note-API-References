---
title: ImageSaveOptions
second_title: Aspose.Note för .NET API-referens
description: Gör det möjligt att ange ytterligare alternativ när du renderar dokumentsidor till bilder.
type: docs
weight: 700
url: /sv/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Gör det möjligt att ange ytterligare alternativ när du renderar dokumentsidor till bilder.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions)(SaveFormat) | Initierar en ny instans av[`ImageSaveOptions`](../imagesaveoptions) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions) { get; set; } | Hämtar eller ställer in alternativ för bildens binarisering. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode) { get; set; } | Hämtar eller sätter[`ColorMode`](./colormode) för utdatabilden. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Hämtar eller ställer in teckensnittets inställningar som ska användas medan de sparas |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Hämtar eller ställer in antalet sidor som ska sparas. Som standard ärMaxValue vilket innebär att alla sidor i dokumentet kommer att renderas. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Hämtar eller ställer in indexet för den första sidan som ska sparas. Som standard är 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality) { get; set; } | Hämtar eller ställer in ett värde som bestämmer kvaliteten på sparad bild. Detta värde skickas till codec som System.Drawing.Imaging.Encoder.Quality parameter. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution) { get; set; } | Hämtar eller ställer in upplösningen för de genererade bilderna, i punkter per tum. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Hämtar formatet som dokumentet sparas i. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression) { get; set; } | Hämtar eller ställer in vilken typ av komprimering som ska användas när genererade bilder sparas i TIFF-formatet. |

### Exempel

Visar hur man sparar ett dokument som bild i Jpeg-format med hjälp av SaveFormat.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Spara dokumentet.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Visar hur du ställer in en bildkvalitet när du sparar dokument som bild i JPEG-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Spara dokumentet.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Visar hur man sparar ett dokument som bild i Bmp-format med hjälp av ImageSaveOptions.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Spara dokumentet.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Visar hur du ställer in en bildupplösning när du sparar dokument som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Spara dokumentet.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Visar hur man sparar ett dokument som gråskalebild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Spara dokumentet som gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Visar hur man sparar ett dokument som bild i Tiff-format med PackBits-komprimering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Spara dokumentet.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Visar hur du sparar anteckningsboken som bild med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

Visar hur man sparar ett dokument som bild i Tiff-format med Jpeg-komprimering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Spara dokumentet.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Visar hur man sparar tillplattad anteckningsbok som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

Visar hur man sparar ett dokument som bild i Tiff-format med hjälp av CCITT Group 3-faxkomprimering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Spara dokumentet.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Visar hur man sparar ett dokument i png-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera ImageSaveOptions-objekt 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Ställ in sidindex
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Spara dokumentet som PNG.
oneFile.Save(dataDir, opts);
```

Visar hur man sparar ett dokument som binär bild med Otsus metod.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Spara dokumentet som gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Visar hur man sparar ett dokument som binär bild med hjälp av fast tröskel.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Spara dokumentet som gif.
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

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
