---
title: PdfSaveOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: Permite especificar opciones adicionales al renderizar páginas de documentos a PDF.
type: docs
weight: 820
url: /es/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Permite especificar opciones adicionales al renderizar páginas de documentos a PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Obtiene o establece la configuración de la fuente que se usará al guardar |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | Obtiene o establece el tipo de compresión aplicada a las imágenes en el archivo PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | Obtiene o establece un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. El valor puede variar de 0 a 100, donde 0 significa la peor calidad pero la compresión máxima y 100 significa la mejor calidad pero la compresión mínima. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Obtiene o establece el número de páginas a guardar. Por defecto esMaxValue lo que significa que se procesarán todas las páginas del documento. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Obtiene o establece el índice de la primera página a guardar. Por defecto es 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | Obtiene o establece el algoritmo utilizado para la división de páginas. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Obtiene el formato en el que se guarda el documento. |

### Ejemplos

Muestra cómo guardar un cuaderno en formato pdf con opciones específicas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Guardar el cuaderno
notebook.Save(dataDir, notebookSaveOptions);
```

Cuando las páginas largas de OneNote se guardan en formato pdf, se dividen en páginas. El ejemplo muestra cómo configurar la lógica de división de objetos ubicados en los saltos de página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// o
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
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

Cuando las páginas largas de OneNote se guardan en formato pdf, se dividen en páginas. El ejemplo muestra cómo configurar la lógica de división de objetos ubicados en los saltos de página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Cargue el documento en Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// O
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Ver también

* class [SaveOptions](../saveoptions)
* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving)
* asamblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
