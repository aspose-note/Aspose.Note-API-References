---
title: Save
second_title: Aspose.Note für .NET-API-Referenz
description: Speichert das OneNote-Dokument in einer Datei.
type: docs
weight: 140
url: /de/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Speichert das OneNote-Dokument in einer Datei.

```csharp
public void Save(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der vollständige Name der Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen vorhanden ist, wird die vorhandene Datei überschrieben. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Die Dokumentstruktur verstößt gegen die Spezifikation. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Das angeforderte Speicherformat wird nicht unterstützt. |

### Beispiele

Zeigt, wie ein Dokument gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Speichert das OneNote-Dokument in einem Stream.

```csharp
public void Save(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der System.IO.Stream, in dem das Dokument gespeichert wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Die Dokumentstruktur verstößt gegen die Spezifikation. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Das angeforderte Speicherformat wird nicht unterstützt. |

### Siehe auch

* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Speichert das OneNote-Dokument in einer Datei im angegebenen Format.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der vollständige Name der Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen vorhanden ist, wird die vorhandene Datei überschrieben. |
| format | SaveFormat | Das Format, in dem das Dokument gespeichert werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Die Dokumentstruktur verstößt gegen die Spezifikation. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Das angeforderte Speicherformat wird nicht unterstützt. |

### Beispiele

Zeigt, wie ein Dokument mithilfe der SaveFormat-Enumeration gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
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

### Siehe auch

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Speichert das OneNote-Dokument in einem Stream im angegebenen Format.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der System.IO.Stream, in dem das Dokument gespeichert wird. |
| format | SaveFormat | Das Format, in dem das Dokument gespeichert werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Die Dokumentstruktur verstößt gegen die Spezifikation. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Das angeforderte Speicherformat wird nicht unterstützt. |

### Beispiele

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

Zeigt, wie ein Dokument in einem Stream gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Spulen Sie die Stream-Position auf Null zurück, damit sie für den nächsten Reader bereit ist.
dstStream.Seek(0, SeekOrigin.Begin);
```

### Siehe auch

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Speichert das OneNote-Dokument unter Verwendung der angegebenen Speicheroptionen in einer Datei.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der vollständige Name der Datei. Wenn bereits eine Datei mit dem angegebenen vollständigen Namen vorhanden ist, wird die vorhandene Datei überschrieben. |
| options | SaveOptions | Gibt die Optionen an, wie das Dokument in der Datei gespeichert wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Die Dokumentstruktur verstößt gegen die Spezifikation. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Das angeforderte Speicherformat wird nicht unterstützt. |

### Beispiele

Zeigt, wie ein Dokument mit OneSaveOptions gespeichert wird.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
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

Zeigt, wie ein Dokument im PDF-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Seitenindex der ersten zu speichernden Seite setzen
                              PageIndex = 0,

                              // Seitenanzahl festlegen
                              PageCount = 1,
                          };

// Dokument als PDF speichern
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Zeigt, wie Sie ein Dokument im PDF-Format mit bestimmten Einstellungen speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // JPEG-Komprimierung verwenden
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualität für JPEG-Komprimierung
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Speichert das OneNote-Dokument unter Verwendung der angegebenen Speicheroptionen in einem Stream.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der System.IO.Stream, in dem das Dokument gespeichert wird. |
| options | SaveOptions | Gibt die Optionen an, wie das Dokument im Stream gespeichert wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Die Dokumentstruktur verstößt gegen die Spezifikation. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Das angeforderte Speicherformat wird nicht unterstützt. |

### Beispiele

Zeigt, wie ein Dokument im PDF-Format mit einer angegebenen Standardschriftart gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Dokument als PDF speichern
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Zeigt, wie ein Dokument im PDF-Format mit Standardschriftart aus einer Datei gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Dokument als PDF speichern
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Zeigt, wie ein Dokument im PDF-Format mit Standardschriftart aus einem Stream gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Dokument als PDF speichern
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Siehe auch

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* namensraum [Aspose.Note](../../document)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
