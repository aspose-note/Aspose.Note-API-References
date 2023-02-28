---
title: Document.Save
second_title: Référence de l'API Aspose.Note pour .NET
description: Document méthode. Enregistre le document OneNote dans un fichier.
type: docs
weight: 140
url: /fr/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Enregistre le document OneNote dans un fichier.

```csharp
public void Save(string fileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | Le nom complet du fichier. Si un fichier avec le nom complet spécifié existe déjà, le fichier existant est écrasé. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | La structure du document viole les spécifications. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Le format d'enregistrement demandé n'est pas pris en charge. |

### Exemples

Montre comment enregistrer un document.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Enregistre le document OneNote dans un flux.

```csharp
public void Save(Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le System.IO.Stream où le document sera enregistré. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | La structure du document viole les spécifications. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Le format d'enregistrement demandé n'est pas pris en charge. |

### Voir également

* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Enregistre le document OneNote dans un fichier au format spécifié.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | Le nom complet du fichier. Si un fichier avec le nom complet spécifié existe déjà, le fichier existant est écrasé. |
| format | SaveFormat | Le format dans lequel enregistrer le document. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | La structure du document viole les spécifications. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Le format d'enregistrement demandé n'est pas pris en charge. |

### Exemples

Montre comment enregistrer un document à l'aide de l'énumération SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Montre comment enregistrer un document au format gif.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### Voir également

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Enregistre le document OneNote dans un flux au format spécifié.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le System.IO.Stream où le document sera enregistré. |
| format | SaveFormat | Le format dans lequel enregistrer le document. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | La structure du document viole les spécifications. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Le format d'enregistrement demandé n'est pas pris en charge. |

### Exemples

Montre comment enregistrer un document au format pdf en utilisant les paramètres par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Montre comment enregistrer un document dans un flux.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Rembobine la position du flux à zéro pour qu'il soit prêt pour le prochain lecteur.
dstStream.Seek(0, SeekOrigin.Begin);
```

Montre comment appliquer le style de thème sombre à un document.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
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

### Voir également

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Enregistre le document OneNote dans un fichier à l'aide des options d'enregistrement spécifiées.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | Le nom complet du fichier. Si un fichier avec le nom complet spécifié existe déjà, le fichier existant est écrasé. |
| options | SaveOptions | Spécifie les options d'enregistrement du document dans le fichier. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | La structure du document viole les spécifications. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Le format d'enregistrement demandé n'est pas pris en charge. |

### Exemples

Montre comment enregistrer un document à l'aide de OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Montre comment enregistrer un document en tant qu'image au format Jpeg à l'aide de SaveFormat.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Enregistre le document.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Montre comment enregistrer un document en tant qu'image au format Bmp à l'aide d'ImageSaveOptions.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Enregistre le document.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Montre comment enregistrer un document au format Pdf avec une mise en page Lettre.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Enregistre le document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Montre comment enregistrer un document au format Pdf avec une mise en page A4 sans limite de hauteur.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Enregistre le document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Montre comment enregistrer un document en tant qu'image en niveaux de gris.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Montre comment enregistrer un document en tant qu'image au format Tiff à l'aide de la compression PackBits.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Enregistre le document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Montre comment enregistrer un document en tant qu'image au format Tiff à l'aide de la compression Jpeg.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Enregistre le document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Montre comment enregistrer un document en tant qu'image au format Tiff à l'aide de la compression de télécopie CCITT Groupe 3.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Enregistre le document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Montre comment enregistrer un document au format pdf.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Définit l'index de la première page à enregistrer
                              PageIndex = 0,

                              // Définir le nombre de pages
                              PageCount = 1,
                          };

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Montre comment enregistrer un document au format pdf en utilisant des paramètres spécifiques.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Utiliser la compression Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualité pour la compression JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Montre comment enregistrer un document en tant qu'image binaire à l'aide de la méthode d'Otsu.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Montre comment enregistrer un document en tant qu'image binaire à l'aide d'un seuil fixe.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Enregistrez le document au format gif.
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

### Voir également

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Enregistre le document OneNote dans un flux à l'aide des options d'enregistrement spécifiées.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le System.IO.Stream où le document sera enregistré. |
| options | SaveOptions | Spécifie les options d'enregistrement du document dans le flux. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | La structure du document viole les spécifications. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Le format d'enregistrement demandé n'est pas pris en charge. |

### Exemples

Montre comment enregistrer un document au format pdf en utilisant la police par défaut spécifiée.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Montre comment enregistrer un document au format pdf en utilisant la police par défaut d'un fichier.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Montre comment enregistrer un document au format pdf en utilisant la police par défaut d'un flux.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Voir également

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


