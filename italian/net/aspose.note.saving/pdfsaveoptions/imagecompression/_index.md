---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note per .NET API Reference
description: PdfSaveOptions proprietà. Ottiene o imposta il tipo di compressione applicato alle immagini nel file PDF.
type: docs
weight: 20
url: /it/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Ottiene o imposta il tipo di compressione applicato alle immagini nel file PDF.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

### Esempi

Mostra come salvare un documento in formato pdf utilizzando impostazioni specifiche.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inizializza l'oggetto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Usa la compressione Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualità per la compressione JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### Guarda anche

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../pdfsaveoptions/)
* assemblea [Aspose.Note](../../../)


