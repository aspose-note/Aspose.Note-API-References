---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note para la referencia de la API de .NET
description: PdfSaveOptions propiedad. Obtiene o establece un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. El valor puede variar de 0 a 100 donde 0 significa la peor calidad pero la compresión máxima y 100 significa la mejor calidad pero la compresión mínima.
type: docs
weight: 30
url: /es/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

Obtiene o establece un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. El valor puede variar de 0 a 100, donde 0 significa la peor calidad pero la compresión máxima y 100 significa la mejor calidad pero la compresión mínima.

```csharp
public int JpegQuality { get; set; }
```

### Observaciones

El valor predeterminado es 90.

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

* class [PdfSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../pdfsaveoptions/)
* asamblea [Aspose.Note](../../../)


