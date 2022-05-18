---
title: Notebook
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 360
url: /net/aspose.note/notebook/
---
## Notebook class

Represents an Aspose.Note notebook.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Constructors

| Name | Description |
| --- | --- |
| [Notebook](notebook)() | Initializes a new instance of the [`Notebook`](../notebook) class. |
| [Notebook](notebook)(Stream) | Initializes a new instance of the [`Notebook`](../notebook) class. Opens an existing OneNote notebook from a stream. |
| [Notebook](notebook)(string) | Initializes a new instance of the [`Notebook`](../notebook) class. Opens an existing OneNote notebook from a file. |
| [Notebook](notebook)(Stream, NotebookLoadOptions) | Initializes a new instance of the [`Notebook`](../notebook) class. Opens an existing OneNote notebook from a stream. Allows to specify additional loading options. |
| [Notebook](notebook)(string, NotebookLoadOptions) | Initializes a new instance of the [`Notebook`](../notebook) class. Opens an existing OneNote notebook from a file. Allows to specify additional options such as a children loading strategy ("lazy"/instant). |

## Properties

| Name | Description |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Gets or sets the color. |
| [Count](../../aspose.note/notebook/count) { get; } | Gets the number of elements contained in the [`Notebook`](../notebook). |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Gets or sets the display name. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Gets file format (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Gets the object's globally unique id. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Gets or sets a value indicating whether the history is enabled. |
| [Item](../../aspose.note/notebook/item) { get; } | Gets notebook child node by the given index. |

## Methods

| Name | Description |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Adds the node to the end of the list. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Get all child nodes by the node type. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Returns an enumerator that iterates through child nodes of the [`Notebook`](../notebook). |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument)(Stream) | Adds a child document node. Opens an existing OneNote document from a stream. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument)(string) | Adds a child document node. Opens an existing OneNote document from a file. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument)(Stream, LoadOptions) | Adds a child document node. Opens an existing OneNote document from a stream. Allows to specify additional load options. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument)(string, LoadOptions) | Adds a child document node. Opens an existing OneNote document from a file. Allows to specify additional load options. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook)(Stream) | Adds a child notebook node. Opens an existing OneNote notebook from a stream. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook)(string) | Adds a child notebook node. Opens an existing OneNote notebook from a file. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook)(Stream, NotebookLoadOptions) | Adds a child notebook node. Opens an existing OneNote notebook from a stream. Allows to specify additional load options. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook)(string, NotebookLoadOptions) | Adds a child notebook node. Opens an existing OneNote notebook from a file. Allows to specify additional load options. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Removes the child node. |
| [Save](../../aspose.note/notebook/save)(Stream) | Saves the OneNote document to a stream. |
| [Save](../../aspose.note/notebook/save)(string) | Saves the OneNote document to a file. |
| [Save](../../aspose.note/notebook/save)(Stream, NotebookSaveOptions) | Saves the OneNote document to a stream using the specified save options. |
| [Save](../../aspose.note/notebook/save)(Stream, SaveFormat) | Saves the OneNote document to a stream in the specified format. |
| [Save](../../aspose.note/notebook/save)(string, NotebookSaveOptions) | Saves the OneNote document to a file using the specified save options. |
| [Save](../../aspose.note/notebook/save)(string, SaveFormat) | Saves the OneNote document to a file in the specified format. |

### Examples

Shows how to save notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Save the Notebook
notebook.Save(dataDir);
```

Shows how to save notebook in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Save the Notebook
notebook.Save(dataDir);
```

Shows how to save notebook as image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Save the Notebook
notebook.Save(dataDir);
```

Shows how to get all text from a notebook.

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

Shows how to save flattened notebook in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Save the Notebook
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Shows how to iterate through documents of a notebook loading them lazily.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// By default children loading is "lazy".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Actual loading of the child document happens only here.
    // Do something with child document
}
```

Shows how to add new section to a notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Append a new child to the Notebook
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Save the Notebook
notebook.Save(dataDir);
```

Shows how to load notebook from a stream.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Shows how to an encrypted notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Shows how to save notebook as image with specified options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
```

Shows how to save flattened notebook as image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
```

Shows how to remove a section from a notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "test.onetoc2");

// Traverse through its child nodes for searching the desired child item
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Remove the Child Item from the Notebook
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Save the Notebook
notebook.Save(dataDir);
```

Shows how to iterate through preloaded documents of a notebook.

```csharp
// By default children loading is "lazy".
// Therefore for instant loading has took place,
// it is necessary to set the NotebookLoadOptions.InstantLoading flag.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// All child documents are already loaded.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Do something with child document
}
```

Shows how to pass through content of a notebook.

```csharp
// The path to the documents directory.
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
            // Do something with child document
        }
        else if (notebookChildNode is Notebook)
        {
            // Do something with child notebook
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### See Also

* interface [INotebookChildNode](../inotebookchildnode)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
