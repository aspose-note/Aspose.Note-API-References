---
title: Page.IsConflictPage
second_title: Aspose.Note for .NET API Reference
description: Page property. Gets or sets a value indicating whether this page is a conflict page
type: docs
weight: 50
url: /net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Gets or sets a value indicating whether this page is a conflict page.

```csharp
public bool IsConflictPage { get; set; }
```

## Remarks

The conflict page arises when two users try to update the same content. In this case the changes of first user are written as usual. But changes of another user can't be merged. So just a copy of page is created and marked as conflict.

At this version the conflicts are resolved in favor of the first user's changes. So if document has conflict pages then they will be shown in history but they will be skipped on saving. It is possible to reset this flag to save this pages in history as usual ones.

Detailed sample of manipulating by conflict page can be found in the online documentation.

## Examples

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

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


