---
title: ImageSaveOptions.Quality
second_title: Aspose.Note para la referencia de la API de .NET
description: ImageSaveOptions propiedad. Obtiene o establece un valor que determina la calidad de la imagen guardada. Este valor se pasa al códec como parámetro System.Drawing.Imaging.Encoder.Quality.
type: docs
weight: 40
url: /es/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Obtiene o establece un valor que determina la calidad de la imagen guardada. Este valor se pasa al códec como parámetro System.Drawing.Imaging.Encoder.Quality.

```csharp
public int Quality { get; set; }
```

### Observaciones

El rango de valores útiles para la categoría de calidad es de 0 a 100. Cuanto menor sea el número especificado, mayor será la compresión y, por lo tanto, menor será la calidad de la imagen. Cero le dará la imagen de menor calidad y 100 la mayor . El valor predeterminado es 90.

### Ejemplos

Muestra cómo establecer una calidad de imagen al guardar un documento como imagen en formato JPEG.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Guarda el documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Muestra cómo guardar un documento como imagen en formato Tiff usando compresión Jpeg.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Guarda el documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### Ver también

* class [ImageSaveOptions](../)
* espacio de nombres [Aspose.Note.Saving](../../imagesaveoptions/)
* asamblea [Aspose.Note](../../../)


