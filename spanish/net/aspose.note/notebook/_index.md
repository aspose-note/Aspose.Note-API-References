---
title: Notebook
second_title: Aspose.Note para la referencia de la API de .NET
description: Representa un cuaderno Aspose.Note.
type: docs
weight: 390
url: /es/net/aspose.note/notebook/
---
## Notebook class

Representa un cuaderno Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Notebook](notebook#constructor)() | Inicializa una nueva instancia del[`Notebook`](../notebook) clase. |
| [Notebook](notebook#constructor_1)(Stream) | Inicializa una nueva instancia del[`Notebook`](../notebook) class. Abre un bloc de notas de OneNote existente desde una secuencia. |
| [Notebook](notebook#constructor_3)(string) | Inicializa una nueva instancia del[`Notebook`](../notebook) class. Abre un bloc de notas de OneNote existente desde un archivo. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | Inicializa una nueva instancia del[`Notebook`](../notebook) class. Abre un bloc de notas de OneNote existente desde una secuencia. Permite especificar opciones de carga adicionales. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | Inicializa una nueva instancia del[`Notebook`](../notebook)class. Abre un bloc de notas de OneNote existente desde un archivo. Permite especificar opciones adicionales, como una estrategia de carga de niños ("lazy"/instant). |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Obtiene o establece el color. |
| [Count](../../aspose.note/notebook/count) { get; } | Obtiene el número de elementos contenidos en el[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Obtiene o establece el nombre para mostrar. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Obtiene el formato de archivo (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Obtiene la identificación única global del objeto. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Obtiene o establece un valor que indica si el historial está habilitado. |
| [Item](../../aspose.note/notebook/item) { get; } | Obtiene el nodo secundario del cuaderno por el índice dado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Agrega el nodo al final de la lista. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Obtener todos los nodos secundarios por tipo de nodo. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Devuelve un enumerador que itera a través de los nodos secundarios del[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde una secuencia. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde un archivo. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde una secuencia. Permite especificar opciones de carga adicionales. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | Agrega un nodo de documento secundario. Abre un documento de OneNote existente desde un archivo. Permite especificar opciones de carga adicionales. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | Agrega un nodo de bloc de notas secundario. Abre un bloc de notas de OneNote existente desde una secuencia. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | Agrega un nodo de bloc de notas secundario. Abre un bloc de notas de OneNote existente desde un archivo. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Agrega un nodo de bloc de notas secundario. Abre un bloc de notas de OneNote existente desde una secuencia. Permite especificar opciones de carga adicionales. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | Agrega un nodo de bloc de notas secundario. Abre un bloc de notas de OneNote existente desde un archivo. Permite especificar opciones de carga adicionales. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Elimina el nodo secundario. |
| [Save](../../aspose.note/notebook/save#save)(Stream) | Guarda el documento de OneNote en una secuencia. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | Guarda el documento de OneNote en un archivo. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | Guarda el documento de OneNote en una secuencia con las opciones de guardado especificadas. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | Guarda el documento de OneNote en una secuencia en el formato especificado. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | Guarda el documento de OneNote en un archivo usando las opciones de guardado especificadas. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | Guarda el documento de OneNote en un archivo con el formato especificado. |

### Ejemplos

Muestra cómo guardar el cuaderno.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Guardar el cuaderno
notebook.Save(dataDir);
```

Muestra cómo guardar el cuaderno en formato pdf.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Guardar el cuaderno
notebook.Save(dataDir);
```

Muestra cómo guardar el cuaderno como imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Guardar el cuaderno
notebook.Save(dataDir);
```

Muestra cómo obtener todo el texto de un bloc de notas.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

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

Muestra cómo iterar a través de documentos de un cuaderno cargándolos con pereza.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Por defecto, la carga de niños es "perezosa".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // La carga real del documento secundario ocurre solo aquí.
    // Hacer algo con el documento secundario
}
```

Muestra cómo agregar una nueva sección a un cuaderno.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Agregar un nuevo hijo al Cuaderno
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Guardar el cuaderno
notebook.Save(dataDir);
```

Muestra cómo cargar un cuaderno desde una secuencia.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Muestra cómo un cuaderno encriptado.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Muestra cómo guardar el cuaderno como imagen con opciones específicas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

Muestra cómo eliminar una sección de un bloc de notas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Atraviesa sus nodos secundarios para buscar el elemento secundario deseado
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Eliminar el elemento secundario del cuaderno
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Guardar el cuaderno
notebook.Save(dataDir);
```

Muestra cómo iterar a través de documentos precargados de un cuaderno.

```csharp
// Por defecto, la carga de niños es "perezosa".
// Por lo tanto, para carga instantánea ha tenido lugar,
// es necesario establecer el indicador NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Todos los documentos secundarios ya están cargados.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Hacer algo con el documento secundario
}
```

Muestra cómo pasar el contenido de un bloc de notas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Hacer algo con el documento secundario
        }
        else if (notebookChildNode is Notebook)
        {
            // Hacer algo con el cuaderno del niño
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* interface [INotebookChildNode](../inotebookchildnode)
* espacio de nombres [Aspose.Note](../../aspose.note)
* asamblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
