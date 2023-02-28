---
title: Enum SaveFormat
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.SaveFormat enum. Indica il formato in cui viene salvato il documento.
type: docs
weight: 540
url: /it/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Indica il formato in cui viene salvato il documento.

```csharp
public enum SaveFormat
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Png | `1` | Specifica che l'output è un file PNG. |
| Bmp | `2` | Specifica che l'output è un file BMP. |
| Jpeg | `3` | Specifica che l'output è un file JPEG. |
| Gif | `4` | Specifica che l'output è un file GIF. |
| Tiff | `5` | Specifica che l'output è un file TIFF. |
| Pdf | `6` | Specifica che l'output è un file PDF. |
| One | `7` | Specifica che l'output è un file OneNote. |
| Html | `8` | Specifica che l'output è un file HTML. |

### Esempi

Mostra come salvare un documento usando l'enumerazione SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Mostra come salvare un documento in formato pdf utilizzando le impostazioni predefinite.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Salva il documento come PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Mostra come salvare un documento come immagine in formato Jpeg utilizzando SaveFormat.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Salva il documento.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Mostra come salvare un documento in formato gif.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Salva il documento come gif.
oneFile.Save(dataDir, SaveFormat.Gif);
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

Mostra come impostare una risoluzione dell'immagine quando si salva il documento come immagine.

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

Mostra come salvare un documento come immagine in formato Tiff utilizzando la compressione PackBits.

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

Mostra come salvare un documento come immagine in formato Tiff utilizzando la compressione Jpeg.

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

* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


