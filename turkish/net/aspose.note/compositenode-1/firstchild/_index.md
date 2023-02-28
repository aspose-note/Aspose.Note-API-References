---
title: CompositeNode1.FirstChild
second_title: Aspose.Note for .NET API Referansı
description: CompositeNode mülk. Bu düğümün ilk alt düğümünü alır.
type: docs
weight: 10
url: /tr/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Bu düğümün ilk alt düğümünü alır.

```csharp
public T FirstChild { get; }
```

### Örnekler

Bir sayfanın çakışma sayfası olup olmadığının nasıl kontrol edileceğini gösterir (yani, OneNote'un otomatik olarak birleştiremediği değişiklikler içerir).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote belgesini yükleyin
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

    // Varsayılan olarak çakışma sayfaları kaydedilirken atlanır.
    // Çakışmasız olarak işaretlerseniz, geçmişe her zamanki gibi kaydedilecektir.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Ayrıca bakınız

* class [CompositeNode&lt;T&gt;](../)
* ad alanı [Aspose.Note](../../compositenode-1/)
* toplantı [Aspose.Note](../../../)


