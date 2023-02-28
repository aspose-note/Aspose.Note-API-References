---
title: CompositeNode1.FirstChild
second_title: Aspose.Note för .NET API-referens
description: CompositeNode fast egendom. Hämtar den första underordnade noden för denna nod.
type: docs
weight: 10
url: /sv/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Hämtar den första underordnade noden för denna nod.

```csharp
public T FirstChild { get; }
```

### Exempel

Visar hur man kontrollerar om en sida är en konfliktsida (dvs. den har ändringar som OneNote inte kunde slå samman automatiskt).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument
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

    // Som standard hoppas konfliktsidor bara över när du sparar.
    // Om det markeras som icke-konflikt kommer det att sparas som vanligt i historiken.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Se även

* class [CompositeNode&lt;T&gt;](../)
* namnutrymme [Aspose.Note](../../compositenode-1/)
* hopsättning [Aspose.Note](../../../)


