---
title: Save
second_title: Aspose.Note per .NET API Reference
description: Salva il documento di OneNote in un file.
type: docs
weight: 140
url: /it/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Salva il documento di OneNote in un file.

```csharp
public void Save(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome completo del file. Se esiste già un file con il nome completo specificato, il file esistente viene sovrascritto. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La struttura del documento viola le specifiche. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Il formato di salvataggio richiesto non è supportato. |

### Esempi

Mostra come salvare un documento.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Guarda anche

* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Salva il documento di OneNote in un flusso.

```csharp
public void Save(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il System.IO.Stream in cui verrà salvato il documento. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La struttura del documento viola le specifiche. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Il formato di salvataggio richiesto non è supportato. |

### Guarda anche

* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Salva il documento di OneNote in un file nel formato specificato.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome completo del file. Se esiste già un file con il nome completo specificato, il file esistente viene sovrascritto. |
| format | SaveFormat | Il formato in cui salvare il documento. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La struttura del documento viola le specifiche. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Il formato di salvataggio richiesto non è supportato. |

### Esempi

Mostra come salvare un documento usando l'enumerazione SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
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

### Guarda anche

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Salva il documento di OneNote in un flusso nel formato specificato.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il System.IO.Stream in cui verrà salvato il documento. |
| format | SaveFormat | Il formato in cui salvare il documento. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La struttura del documento viola le specifiche. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Il formato di salvataggio richiesto non è supportato. |

### Esempi

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

Mostra come salvare un documento in uno stream.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Riavvolgi la posizione del flusso a zero in modo che sia pronto per il prossimo lettore.
dstStream.Seek(0, SeekOrigin.Begin);
```

### Guarda anche

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Salva il documento di OneNote in un file utilizzando le opzioni di salvataggio specificate.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome completo del file. Se esiste già un file con il nome completo specificato, il file esistente viene sovrascritto. |
| options | SaveOptions | Specifica le opzioni di salvataggio del documento nel file. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La struttura del documento viola le specifiche. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Il formato di salvataggio richiesto non è supportato. |

### Esempi

Mostra come salvare un documento utilizzando OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Mostra come salvare un documento come immagine in formato Jpeg usando SaveFormat.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Salva il documento.
oneFile.Save(dataDir, SaveFormat.Jpeg);
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

Mostra come salvare un documento come immagine in formato Tiff usando la compressione PackBits.

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

Mostra come salvare un documento come immagine in formato Tiff usando la compressione Jpeg.

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

Mostra come salvare un documento in formato pdf.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Imposta l'indice della prima pagina da salvare
                              PageIndex = 0,

                              // Imposta il conteggio delle pagine
                              PageCount = 1,
                          };

// Salva il documento come PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Mostra come salvare un documento in formato pdf utilizzando impostazioni specifiche.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Usa la compressione JPEG
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualità per la compressione JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Salva il documento di OneNote in un flusso utilizzando le opzioni di salvataggio specificate.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il System.IO.Stream in cui verrà salvato il documento. |
| options | SaveOptions | Specifica le opzioni di salvataggio del documento nello stream. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La struttura del documento viola le specifiche. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | Il formato di salvataggio richiesto non è supportato. |

### Esempi

Mostra come salvare un documento in formato pdf utilizzando il carattere predefinito specificato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Salva il documento come PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Mostra come salvare un documento in formato pdf utilizzando il carattere predefinito da un file.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Salva il documento come PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Mostra come salvare un documento in formato pdf utilizzando il carattere predefinito da uno stream.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Salva il documento come PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Guarda anche

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* spazio dei nomi [Aspose.Note](../../document)
* assemblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
