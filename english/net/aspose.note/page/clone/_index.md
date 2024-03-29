---
title: Page.Clone
second_title: Aspose.Note for .NET API Reference
description: Page method. Clones the page
type: docs
weight: 140
url: /net/aspose.note/page/clone/
---
## Page.Clone method

Clones the page.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cloneHistory | Boolean | Specifies if page's history should be cloned.. |

### Return Value

A clone of the page.

## Examples

Shows how to push current version of a page to history.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document and get first child           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Shows how to clone a page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Clone into new document without history
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Clone into new document with history
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### See Also

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


