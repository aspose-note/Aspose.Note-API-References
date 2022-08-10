---
title: Save
second_title: Aspose.Note para la referencia de la API de .NET
description: Guarda el documento de OneNote en un archivo.
type: docs
weight: 140
url: /es/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Guarda el documento de OneNote en un archivo.

```csharp
public void Save(string fileName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, se sobrescribe el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La estructura del documento infringe la especificación. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | El formato de guardado solicitado no es compatible. |

### Ejemplos

Muestra cómo guardar un documento.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Ver también

* class [Document](../../document)
* espacio de nombres [Aspose.Note](../../document)
* asamblea [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Guarda el documento de OneNote en una secuencia.

```csharp
public void Save(Stream stream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El System.IO.Stream donde se guardará el documento. |

### Excepciones

| excepción | condición |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La estructura del documento infringe la especificación. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | El formato de guardado solicitado no es compatible. |

### Ver también

* class [Document](../../document)
* espacio de nombres [Aspose.Note](../../document)
* asamblea [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Guarda el documento de OneNote en un archivo con el formato especificado.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, se sobrescribe el archivo existente. |
| format | SaveFormat | El formato en el que guardar el documento. |

### Excepciones

| excepción | condición |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La estructura del documento infringe la especificación. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | El formato de guardado solicitado no es compatible. |

### Ejemplos

Muestra cómo guardar un documento mediante la enumeración SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Muestra cómo guardar un documento en formato gif.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Guarda el documento como gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### Ver también

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* espacio de nombres [Aspose.Note](../../document)
* asamblea [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Guarda el documento de OneNote en una secuencia en el formato especificado.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El System.IO.Stream donde se guardará el documento. |
| format | SaveFormat | El formato en el que guardar el documento. |

### Excepciones

| excepción | condición |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La estructura del documento infringe la especificación. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | El formato de guardado solicitado no es compatible. |

### Ejemplos

Muestra cómo guardar un documento en formato pdf utilizando la configuración predeterminada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Guarda el documento como PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Muestra cómo guardar un documento en una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Rebobinar la posición de la transmisión a cero para que esté lista para el próximo lector.
dstStream.Seek(0, SeekOrigin.Begin);
```

### Ver también

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* espacio de nombres [Aspose.Note](../../document)
* asamblea [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Guarda el documento de OneNote en un archivo usando las opciones de guardado especificadas.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | El nombre completo del archivo. Si ya existe un archivo con el nombre completo especificado, se sobrescribe el archivo existente. |
| options | SaveOptions | Especifica las opciones de cómo se guarda el documento en el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La estructura del documento infringe la especificación. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | El formato de guardado solicitado no es compatible. |

### Ejemplos

Muestra cómo guardar un documento usando OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Muestra cómo guardar un documento como imagen en formato Jpeg usando SaveFormat.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Guarda el documento.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Muestra cómo guardar un documento como imagen en formato Bmp usando ImageSaveOptions.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Guarda el documento.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Muestra cómo guardar un documento como imagen en escala de grises.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Guarda el documento como gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

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

Muestra cómo guardar un documento en formato pdf.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inicializa el objeto PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Establecer el índice de página de la primera página que se guardará
                              PageIndex = 0,

                              // Establecer el número de páginas
                              PageCount = 1,
                          };

// Guarda el documento como PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

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

Muestra cómo guardar un documento como imagen binaria usando el método de Otsu.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Guarda el documento como gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Muestra cómo guardar un documento como imagen binaria utilizando un umbral fijo.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Guarda el documento como gif.
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

### Ver también

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* espacio de nombres [Aspose.Note](../../document)
* asamblea [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Guarda el documento de OneNote en una secuencia con las opciones de guardado especificadas.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El System.IO.Stream donde se guardará el documento. |
| options | SaveOptions | Especifica las opciones de cómo se guarda el documento en flujo. |

### Excepciones

| excepción | condición |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | La estructura del documento infringe la especificación. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | El formato de guardado solicitado no es compatible. |

### Ejemplos

Muestra cómo guardar un documento en formato pdf utilizando la fuente predeterminada especificada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Guarda el documento como PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Muestra cómo guardar un documento en formato pdf utilizando la fuente predeterminada de un archivo.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Guarda el documento como PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Muestra cómo guardar un documento en formato pdf utilizando la fuente predeterminada de una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Guarda el documento como PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Ver también

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* espacio de nombres [Aspose.Note](../../document)
* asamblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
