---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note voor .NET API-referentie
description: PdfSaveOptions eigendom. Hiermee wordt een waarde opgehaald of ingesteld die de kwaliteit van de JPEGafbeeldingen in een PDFdocument bepaalt. De waarde kan variëren van 0 tot 100 waarbij 0 de slechtste kwaliteit maar maximale compressie betekent en 100 de beste kwaliteit maar minimale compressie betekent.
type: docs
weight: 30
url: /nl/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

Hiermee wordt een waarde opgehaald of ingesteld die de kwaliteit van de JPEG-afbeeldingen in een PDF-document bepaalt. De waarde kan variëren van 0 tot 100, waarbij 0 de slechtste kwaliteit maar maximale compressie betekent en 100 de beste kwaliteit maar minimale compressie betekent.

```csharp
public int JpegQuality { get; set; }
```

### Opmerkingen

De standaardwaarde is 90.

### Voorbeelden

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

### Zie ook

* class [PdfSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../pdfsaveoptions/)
* montage [Aspose.Note](../../../)


