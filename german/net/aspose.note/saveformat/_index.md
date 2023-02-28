---
title: Enum SaveFormat
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.SaveFormat opsomming. Gibt das Format an in dem das Dokument gespeichert wird.
type: docs
weight: 540
url: /de/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Gibt das Format an, in dem das Dokument gespeichert wird.

```csharp
public enum SaveFormat
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Png | `1` | Gibt an, dass die Ausgabe eine PNG-Datei ist. |
| Bmp | `2` | Gibt an, dass die Ausgabe eine BMP-Datei ist. |
| Jpeg | `3` | Gibt an, dass die Ausgabe eine JPEG-Datei ist. |
| Gif | `4` | Gibt an, dass die Ausgabe eine GIF-Datei ist. |
| Tiff | `5` | Gibt an, dass die Ausgabe eine TIFF-Datei ist. |
| Pdf | `6` | Gibt an, dass die Ausgabe eine PDF-Datei ist. |
| One | `7` | Gibt an, dass die Ausgabe eine OneNote-Datei ist. |
| Html | `8` | Gibt an, dass die Ausgabe eine HTML-Datei ist. |

### Beispiele

Zeigt, wie ein Dokument mithilfe der SaveFormat-Enumeration gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Zeigt, wie Sie ein Dokument im PDF-Format mit Standardeinstellungen speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dokument als PDF speichern
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Zeigt, wie ein Dokument mit SaveFormat als Bild im Jpeg-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Speichern Sie das Dokument.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Zeigt, wie ein Dokument im gif-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Speichern Sie das Dokument als gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Zeigt, wie eine Bildqualität eingestellt wird, wenn ein Dokument als Bild im JPEG-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Speichern Sie das Dokument.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Zeigt, wie ein Dokument mit ImageSaveOptions als Bild im BMP-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Speichern Sie das Dokument.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Zeigt, wie eine Bildauflösung eingestellt wird, wenn ein Dokument als Bild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Speichern Sie das Dokument.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Zeigt, wie ein Dokument als Graustufenbild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Speichern Sie das Dokument als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Zeigt, wie ein Dokument als Bild im Tiff-Format mit PackBits-Komprimierung gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Speichern Sie das Dokument.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Zeigt, wie ein Dokument als Bild im Tiff-Format mit JPEG-Komprimierung gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Speichern Sie das Dokument.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Zeigt, wie ein Dokument als Bild im Tiff-Format mit CCITT Group 3-Faxkomprimierung gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Speichern Sie das Dokument.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Zeigt, wie ein Dokument mit der Methode von Otsu als Binärbild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Speichern Sie das Dokument als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Zeigt, wie ein Dokument als Binärbild mit festem Schwellenwert gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Speichern Sie das Dokument als gif.
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

### Siehe auch

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


