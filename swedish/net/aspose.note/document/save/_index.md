---
title: Save
second_title: Aspose.Note för .NET API-referens
description: Sparar OneNote-dokumentet till en fil.
type: docs
weight: 140
url: /sv/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Sparar OneNote-dokumentet till en fil.

```csharp
public void Save(string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |

### Undantag

| undantag | skick |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Dokumentstrukturen bryter mot specifikationerna. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Det begärda sparformatet stöds inte. |

### Exempel

Visar hur man sparar ett dokument.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Sparar OneNote-dokumentet i en ström.

```csharp
public void Save(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | System.IO.Stream där dokumentet kommer att sparas. |

### Undantag

| undantag | skick |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Dokumentstrukturen bryter mot specifikationerna. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Det begärda sparformatet stöds inte. |

### Se även

* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Sparar OneNote-dokumentet till en fil i det angivna formatet.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |
| format | SaveFormat | Formatet som dokumentet ska sparas i. |

### Undantag

| undantag | skick |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Dokumentstrukturen bryter mot specifikationerna. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Det begärda sparformatet stöds inte. |

### Exempel

Visar hur man sparar ett dokument med hjälp av SaveFormat-uppräkning.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
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

### Se även

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Sparar OneNote-dokumentet i en ström i det angivna formatet.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | System.IO.Stream där dokumentet kommer att sparas. |
| format | SaveFormat | Formatet som dokumentet ska sparas i. |

### Undantag

| undantag | skick |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Dokumentstrukturen bryter mot specifikationerna. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Det begärda sparformatet stöds inte. |

### Exempel

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

Visar hur man sparar ett dokument i en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Spola tillbaka streampositionen till noll så att den är redo för nästa läsare.
dstStream.Seek(0, SeekOrigin.Begin);
```

### Se även

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Sparar OneNote-dokumentet till en fil med de angivna sparalternativen.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Det fullständiga namnet för filen. Om en fil med det angivna fullständiga namnet redan finns, skrivs den befintliga filen över. |
| options | SaveOptions | Anger alternativen hur dokumentet sparas i filen. |

### Undantag

| undantag | skick |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Dokumentstrukturen bryter mot specifikationerna. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Det begärda sparformatet stöds inte. |

### Exempel

Visar hur man sparar ett dokument med OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
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

Visar hur man sparar ett dokument i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ställ in sidindex för första sidan som ska sparas
                              PageIndex = 0,

                              // Ställ in sidantal
                              PageCount = 1,
                          };

// Spara dokumentet som PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Visar hur man sparar ett dokument i pdf-format med specifika inställningar.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Använd Jpeg-komprimering
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kvalitet för JPEG-komprimering
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Sparar OneNote-dokumentet i en ström med de angivna sparalternativen.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | System.IO.Stream där dokumentet kommer att sparas. |
| options | SaveOptions | Anger alternativen för hur dokumentet sparas i stream. |

### Undantag

| undantag | skick |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Dokumentstrukturen bryter mot specifikationerna. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Det begärda sparformatet stöds inte. |

### Exempel

Visar hur man sparar ett dokument i pdf-format med angivet standardteckensnitt.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Spara dokumentet som PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Visar hur man sparar ett dokument i pdf-format med standardteckensnitt från en fil.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Spara dokumentet som PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Visar hur man sparar ett dokument i pdf-format med standardteckensnitt från en ström.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Spara dokumentet som PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Se även

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* namnutrymme [Aspose.Note](../../document)
* hopsättning [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
