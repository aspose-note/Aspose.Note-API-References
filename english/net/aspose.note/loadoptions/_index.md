---
title: Class LoadOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.LoadOptions class. Options used to load a document
type: docs
weight: 380
url: /net/aspose.note/loadoptions/
---
## LoadOptions class

Options used to load a document.

```csharp
public class LoadOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LoadOptions](loadoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | Gets or sets a password for the encrypted document content. Value is ignored in case the document is not password protected. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | Gets or sets a value indicating whether a document loader should ignore the history. Use this option to decrease memory and CPU usage. Default value is `true`. |

## Examples

Shows how to an encrypted document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
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

Shows how to get page's history.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Get first page
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### See Also

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


