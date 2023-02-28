---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions clase. Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular y proporciona opciones de guardado comunes para todos los nodos secundarios del documento.
type: docs
weight: 800
url: /es/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Una clase base abstracta que representa las opciones de guardado del cuaderno para un formato particular y proporciona opciones de guardado comunes para todos los nodos secundarios del documento.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Parámetro | Descripción |
| --- | --- |
| TDocumentSaveOptions | Las opciones de guardado para todos los documentos secundarios de la libreta. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Obtiene o establece un valor que indica si los documentos secundarios deben guardarse explícitamente. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Obtiene o establece las opciones de guardado para todos los documentos secundarios de la libreta. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Obtiene o establece un valor que indica si la jerarquía secundaria del cuaderno se guarda plana. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Obtiene el formato en el que se guarda el cuaderno. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Obtiene las opciones de guardado para todos los documentos secundarios de la libreta. |

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

### Ver también

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* espacio de nombres [Aspose.Note.Saving](../../aspose.note.saving/)
* asamblea [Aspose.Note](../../)


