---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note para la referencia de la API de .NET
description: PdfSaveOptions propiedad. Obtiene o establece el tipo de compresión aplicada a las imágenes en el archivo PDF.
type: docs
weight: 20
url: /es/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Obtiene o establece el tipo de compresión aplicada a las imágenes en el archivo PDF.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

### Ejemplos

Muestra cómo guardar un documento en formato pdf usando configuraciones específicas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inicializa el objeto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Usar compresión JPEG
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Calidad para compresión JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### Ver también

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../pdfsaveoptions/)
* asamblea [Aspose.Note](../../../)


