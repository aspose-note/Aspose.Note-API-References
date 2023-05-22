---
title: Document.GetPageHistory
second_title: Aspose.Note for .NET API Reference
description: Document method. Gets the PageHistory which contains full history for each page presented in a document the earliest at index 0. The current page revision can be accessed as Current and contained separately from collection of historical versions
type: docs
weight: 100
url: /net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Gets the [`PageHistory`](../../pagehistory/) which contains full history for each page presented in a document (the earliest at index 0). The current page revision can be accessed as [`Current`](../../pagehistory/current/) and contained separately from collection of historical versions.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Parameter | Type | Description |
| --- | --- | --- |
| page | Page | The current revision of a page. |

### Return Value

The [`PageHistory`](../../pagehistory/).

## Examples

Shows how to restore previous version of a page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document and get first child           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Shows how to edit page's history.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document and get first child           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Shows how to check if a page is a conflict page(i.e. it has changes that OneNote couldn't automatically merge).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // By default conflict pages are just skipped on saving.
    // If mark it as non-conflict then it will be saved as usual one in the history.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### See Also

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


