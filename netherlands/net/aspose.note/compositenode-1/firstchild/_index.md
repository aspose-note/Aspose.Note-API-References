---
title: CompositeNode1.FirstChild
second_title: Aspose.Note voor .NET API-referentie
description: CompositeNode eigendom. Haalt het eerste onderliggende knooppunt van dit knooppunt op.
type: docs
weight: 10
url: /nl/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Haalt het eerste onderliggende knooppunt van dit knooppunt op.

```csharp
public T FirstChild { get; }
```

### Voorbeelden

Laat zien hoe u kunt controleren of een pagina een conflictpagina is (dwz dat deze wijzigingen bevat die OneNote niet automatisch kan samenvoegen).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
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

    // Standaard worden conflictpagina's gewoon overgeslagen bij het opslaan.
    // Als u het als niet-conflict markeert, wordt het zoals gebruikelijk in de geschiedenis opgeslagen.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Zie ook

* class [CompositeNode&lt;T&gt;](../)
* naamruimte [Aspose.Note](../../compositenode-1/)
* montage [Aspose.Note](../../../)


