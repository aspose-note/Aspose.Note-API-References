---
title: LoadOptions.LoadHistory
second_title: Aspose.Note for .NET API Reference
description: LoadOptions property. Gets or sets a value indicating whether a document loader should ignore the history. Use this option to decrease memory and CPU usage. Default value is true
type: docs
weight: 30
url: /net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Gets or sets a value indicating whether a document loader should ignore the history. Use this option to decrease memory and CPU usage. Default value is `true`.

```csharp
public bool LoadHistory { get; set; }
```

## Examples

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

* class [LoadOptions](../)
* namespace [Aspose.Note](../../loadoptions/)
* assembly [Aspose.Note](../../../)


