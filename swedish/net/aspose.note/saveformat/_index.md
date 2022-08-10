---
title: SaveFormat
second_title: Aspose.Note för .NET API-referens
description: Indikerar formatet som dokumentet har sparats i.
type: docs
weight: 520
url: /sv/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Indikerar formatet som dokumentet har sparats i.

```csharp
public enum SaveFormat
```

### Värderingar

| namn | Värde | Beskrivning |
| --- | --- | --- |
| Png | `1` | Anger att utdata är en PNG-fil. |
| Bmp | `2` | Anger att utdata är en BMP-fil. |
| Jpeg | `3` | Anger att utdata är en JPEG-fil. |
| Gif | `4` | Anger att utdata är en GIF-fil. |
| Tiff | `5` | Anger att utdata är en TIFF-fil. |
| Pdf | `6` | Anger att utdata är en PDF-fil. |
| One | `7` | Anger att utdata är en OneNote-fil. |
| Html | `8` | Anger att utdata är en HTML-fil. |

### Exempel

Visar hur man sparar ett dokument med hjälp av SaveFormat-uppräkning.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Visar hur man sparar ett dokument i pdf-format med standardinställningar.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Spara dokumentet som PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

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

Visar hur man sparar ett dokument i gif-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Spara dokumentet som gif.
oneFile.Save(dataDir, SaveFormat.Gif);
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

* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
