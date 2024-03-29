---
title: CompositeNode1.FirstChild
second_title: Aspose.Note for .NET API Reference
description: CompositeNode property. Gets the first child node of this node
type: docs
weight: 10
url: /net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Gets the first child node of this node.

```csharp
public T FirstChild { get; }
```

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

* class [CompositeNode&lt;T&gt;](../)
* namespace [Aspose.Note](../../compositenode-1/)
* assembly [Aspose.Note](../../../)


