---
title: Class NotebookSaveOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Saving.NotebookSaveOptions clase. Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular.
type: docs
weight: 790
url: /es/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular.

```csharp
public abstract class NotebookSaveOptions
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Obtiene o establece un valor que indica si los documentos secundarios deben guardarse explícitamente. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Obtiene o establece un valor que indica si la jerarquía secundaria del cuaderno se guarda plana. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Obtiene el formato en el que se guarda el cuaderno. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Obtiene las opciones de guardado para todos los documentos secundarios de la libreta. |

### Ejemplos

Muestra cómo guardar un cuaderno aplanado en formato pdf.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Guardar el cuaderno
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

Muestra cómo guardar un cuaderno aplanado como imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Guardar el cuaderno
notebook.Save(dataDir, notebookSaveOptions);
```

### Ver también

* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving/)
* asamblea [Aspose.Note](../../)


