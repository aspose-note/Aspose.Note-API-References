---
title: Save
second_title: Aspose.Note for .NET API Reference
description: Saves the OneNote document to a file.
type: docs
weight: 140
url: /net/aspose.note/document/save/
---
## Save(string) {#save_3}

Saves the OneNote document to a file.

```csharp
public void Save(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Requested save format is not supported. |

### Examples

Shows how to save a document.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### See Also

* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Saves the OneNote document to a stream.

```csharp
public void Save(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The System.IO.Stream where the document will be saved. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Requested save format is not supported. |

### See Also

* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Saves the OneNote document to a file in the specified format.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| format | SaveFormat | The format in which to save the document. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Requested save format is not supported. |

### Examples

Shows how to save a document using SaveFormat enumeration.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Shows how to save a document in gif format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Save the document as gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### See Also

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Saves the OneNote document to a stream in the specified format.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The System.IO.Stream where the document will be saved. |
| format | SaveFormat | The format in which to save the document. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Requested save format is not supported. |

### Examples

Shows how to save a document in pdf format using default settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Save the document as PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Shows how to save a document to a stream.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Rewind the stream position back to zero so it is ready for next reader.
dstStream.Seek(0, SeekOrigin.Begin);
```

Shows how to apply Dark theme style to a Document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### See Also

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Saves the OneNote document to a file using the specified save options.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| options | SaveOptions | Specifies the options how the document is saved in file. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Requested save format is not supported. |

### Examples

Shows how to save a document using OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Shows how to save a document as image in Jpeg format using SaveFormat.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Save the document.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Shows how to save a document as image in Bmp format using ImageSaveOptions.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Save the document.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Shows how to save a document in Pdf format with Letter page layout.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Save the document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Shows how to save a document in Pdf format with A4 page layout without height limit.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Save the document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Shows how to save a document as grayscale image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Save the document as gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Shows how to save a document as image in Tiff format using PackBits compression.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Save the document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Shows how to save a document as image in Tiff format using Jpeg compression.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Save the document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Shows how to save a document as image in Tiff format using CCITT Group 3 fax compression.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Save the document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Shows how to save a document in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Set page index of first page to be saved
                              PageIndex = 0,

                              // Set page count
                              PageCount = 1,
                          };

// Save the document as PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Shows how to save a document in pdf format using specific settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Use Jpeg compression
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Quality for JPEG compression
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Shows how to save a document as binary image using Otsu's method.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Save the document as gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Shows how to save a document as binary image using fixed threshold.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Save the document as gif.
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

### See Also

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Saves the OneNote document to a stream using the specified save options.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The System.IO.Stream where the document will be saved. |
| options | SaveOptions | Specifies the options how the document is saved in stream. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Requested save format is not supported. |

### Examples

Shows how to save a document in pdf format using specified default font.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Save the document as PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Shows how to save a document in pdf format using default font from a file.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Save the document as PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Shows how to save a document in pdf format using default font from a stream.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Save the document as PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### See Also

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* namespace [Aspose.Note](../../document)
* assembly [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
