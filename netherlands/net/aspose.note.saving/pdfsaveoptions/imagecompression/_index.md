---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note voor .NET API-referentie
description: PdfSaveOptions eigendom. Hiermee wordt het type compressie dat wordt toegepast op afbeeldingen in het PDFbestand opgehaald of ingesteld.
type: docs
weight: 20
url: /nl/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Hiermee wordt het type compressie dat wordt toegepast op afbeeldingen in het PDF-bestand opgehaald of ingesteld.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../pdfsaveoptions/)
* montage [Aspose.Note](../../../)


