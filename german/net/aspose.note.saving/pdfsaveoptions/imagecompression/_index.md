---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note für .NET-API-Referenz
description: PdfSaveOptions eigendom. Ruft den auf Bilder in der PDFDatei angewendeten Komprimierungstyp ab oder legt ihn fest.
type: docs
weight: 20
url: /de/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Ruft den auf Bilder in der PDF-Datei angewendeten Komprimierungstyp ab oder legt ihn fest.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../pdfsaveoptions/)
* Montage [Aspose.Note](../../../)


