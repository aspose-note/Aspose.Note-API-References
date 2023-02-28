---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note för .NET API-referens
description: PdfSaveOptions fast egendom. Hämtar eller ställer in typen av komprimering som tillämpas på bilder i PDFfilen.
type: docs
weight: 20
url: /sv/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Hämtar eller ställer in typen av komprimering som tillämpas på bilder i PDF-filen.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

### Exempel

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

### Se även

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../pdfsaveoptions/)
* hopsättning [Aspose.Note](../../../)


