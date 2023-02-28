---
title: Document.Save
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Slaat het OneNotedocument op in een bestand.
type: docs
weight: 140
url: /nl/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Slaat het OneNote-document op in een bestand.

```csharp
public void Save(string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De volledige naam van het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | De documentstructuur is in strijd met de specificatie. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Gevraagde opslagindeling wordt niet ondersteund. |

### Voorbeelden

Laat zien hoe u een document opslaat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Slaat het OneNote-document op in een stream.

```csharp
public void Save(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De System.IO.Stream waar het document wordt opgeslagen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | De documentstructuur is in strijd met de specificatie. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Gevraagde opslagindeling wordt niet ondersteund. |

### Zie ook

* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Slaat het OneNote-document op in een bestand in de opgegeven indeling.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De volledige naam van het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |
| format | SaveFormat | De indeling waarin het document moet worden opgeslagen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | De documentstructuur is in strijd met de specificatie. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Gevraagde opslagindeling wordt niet ondersteund. |

### Voorbeelden

Laat zien hoe u een document kunt opslaan met behulp van SaveFormat-opsomming.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Laat zien hoe je een document opslaat in gif-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Sla het document op als gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### Zie ook

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Slaat het OneNote-document op in een stream in de opgegeven indeling.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De System.IO.Stream waar het document wordt opgeslagen. |
| format | SaveFormat | De indeling waarin het document moet worden opgeslagen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | De documentstructuur is in strijd met de specificatie. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Gevraagde opslagindeling wordt niet ondersteund. |

### Voorbeelden

Laat zien hoe u een document in pdf-indeling kunt opslaan met standaardinstellingen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Sla het document op als PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Laat zien hoe u een document opslaat in een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Spoel de streampositie terug naar nul zodat deze klaar is voor de volgende lezer.
dstStream.Seek(0, SeekOrigin.Begin);
```

Laat zien hoe u de donkere themastijl toepast op een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
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

### Zie ook

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Slaat het OneNote-document op in een bestand met de opgegeven opslagopties.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De volledige naam van het bestand. Als er al een bestand met de opgegeven volledige naam bestaat, wordt het bestaande bestand overschreven. |
| options | SaveOptions | Specificeert de opties hoe het document wordt opgeslagen in bestand. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | De documentstructuur is in strijd met de specificatie. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Gevraagde opslagindeling wordt niet ondersteund. |

### Voorbeelden

Laat zien hoe u een document kunt opslaan met behulp van OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

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

Laat zien hoe u een document in pdf-indeling kunt opslaan met de pagina-indeling Letter.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Sla het document op.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Laat zien hoe u een document opslaat in Pdf-formaat met A4-paginalay-out zonder hoogtebeperking.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Sla het document op.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
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

Laat zien hoe u een document opslaat in pdf-formaat.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Stel de pagina-index in van de eerste pagina die moet worden opgeslagen
                              PageIndex = 0,

                              // Stel het aantal pagina's in
                              PageCount = 1,
                          };

// Sla het document op als PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Laat zien hoe u een document in pdf-formaat kunt opslaan met behulp van specifieke instellingen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialiseer het PdfSaveOptions-object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Gebruik JPEG-compressie
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kwaliteit voor JPEG-compressie
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Slaat het OneNote-document op in een stream met behulp van de opgegeven opslagopties.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De System.IO.Stream waar het document wordt opgeslagen. |
| options | SaveOptions | Specificeert de opties hoe het document wordt opgeslagen in stream. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | De documentstructuur is in strijd met de specificatie. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Gevraagde opslagindeling wordt niet ondersteund. |

### Voorbeelden

Laat zien hoe u een document in pdf-indeling kunt opslaan met het opgegeven standaardlettertype.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Sla het document op als PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Laat zien hoe u een document in pdf-indeling opslaat met het standaardlettertype uit een bestand.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Sla het document op als PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Laat zien hoe u een document in pdf-indeling opslaat met het standaardlettertype van een stream.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Sla het document op als PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Zie ook

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


