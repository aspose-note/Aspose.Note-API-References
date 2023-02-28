---
title: CompositeNode1.FirstChild
second_title: Справочник по API Aspose.Note для .NET
description: CompositeNode свойство. Получает первый дочерний узел этого узла.
type: docs
weight: 10
url: /ru/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Получает первый дочерний узел этого узла.

```csharp
public T FirstChild { get; }
```

### Примеры

Показывает, как проверить, является ли страница конфликтующей (т. е. имеет ли она изменения, которые OneNote не может автоматически объединить).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote
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

    // По умолчанию конфликтующие страницы просто пропускаются при сохранении.
    // Если отметить его как неконфликтный, то он будет сохранен как обычный в истории.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Смотрите также

* class [CompositeNode&lt;T&gt;](../)
* пространство имен [Aspose.Note](../../compositenode-1/)
* сборка [Aspose.Note](../../../)


