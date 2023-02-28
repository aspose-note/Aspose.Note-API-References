---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: NotebookSaveOptions propiedad. Obtiene o establece las opciones de guardado para todos los documentos secundarios de la libreta.
type: docs
weight: 10
url: /es/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Obtiene o establece las opciones de guardado para todos los documentos secundarios de la libreta.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* espacio de nombres [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* asamblea [Aspose.Note](../../../)


