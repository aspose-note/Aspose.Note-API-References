---
title: Class ImageSaveOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.ImageSaveOptions klas. Ermöglicht das Festlegen zusätzlicher Optionen beim Rendern von Dokumentseiten in Bilder.
type: docs
weight: 720
url: /de/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Ermöglicht das Festlegen zusätzlicher Optionen beim Rendern von Dokumentseiten in Bilder.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Initialisiert eine neue Instanz von`ImageSaveOptions` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Ruft Optionen für die Binarisierung von Bildern ab oder legt sie fest. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Holt oder setzt[`ColorMode`](./colormode/) für das Ausgabebild. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Ruft die beim Speichern zu verwendenden Schrifteinstellungen ab oder legt sie fest |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. Standardmäßig istMaxValue , was bedeutet, dass alle Seiten des Dokuments gerendert werden. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der die Qualität des gespeicherten Bildes bestimmt. Dieser Wert wird als System.Drawing.Imaging.Encoder.Quality-Parameter an den Codec übergeben. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Ruft die Auflösung für die generierten Bilder in Punkten pro Zoll ab oder legt sie fest. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Ruft das Format ab, in dem das Dokument gespeichert ist. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Ruft den Komprimierungstyp ab oder legt ihn fest, der beim Speichern generierter Bilder im TIFF-Format verwendet werden soll. |

### Beispiele

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

Zeigt, wie Notizbuch als Bild mit bestimmten Optionen gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Speichern Sie das Notizbuch
notebook.Save(dataDir, notebookSaveOptions);
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

Zeigt, wie ein reduziertes Notizbuch als Bild gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ein OneNote-Notizbuch laden
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Speichern Sie das Notizbuch
notebook.Save(dataDir, notebookSaveOptions);
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

Zeigt, wie ein Dokument im PNG-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions-Objekt initialisieren 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Seitenindex setzen
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Speichern Sie das Dokument als PNG.
oneFile.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


