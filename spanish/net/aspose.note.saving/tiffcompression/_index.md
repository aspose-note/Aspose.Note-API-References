---
title: Enum TiffCompression
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Saving.TiffCompression enumeración. Especifica qué tipo de compresión usar al guardar un documento en formato TIFF.
type: docs
weight: 880
url: /es/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Especifica qué tipo de compresión usar al guardar un documento en formato TIFF.

```csharp
public enum TiffCompression
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `1` | No especifica compresión. |
| Rle | `2` | Especifica la compresión RLE. |
| Ccitt3 | `3` | Especifica la codificación de fax CCITT Grupo 3. |
| Ccitt4 | `4` | Especifica la codificación de fax CCITT Grupo 4. |
| Lzw | `5` | Especifica la compresión LZW. |
| PackBits | `32773` | Especifica la compresión RLE de Macintosh. |
| Jpeg | `7` | Especifica la compresión de compresión JPEG DCT. |

### Ejemplos

Muestra cómo guardar un documento como imagen en formato Tiff utilizando la compresión PackBits.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Guarda el documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
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

Muestra cómo guardar un documento como imagen en formato Tiff utilizando la compresión de fax CCITT Grupo 3.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Guarda el documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### Ver también

* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving/)
* asamblea [Aspose.Note](../../)


