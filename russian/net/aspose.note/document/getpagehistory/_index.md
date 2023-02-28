---
title: Document.GetPageHistory
second_title: Справочник по API Aspose.Note для .NET
description: Document метод. ПолучаетPageHistory который содержит полную историю для каждой страницы представленной в документе самая ранняя с индексом 0. Доступ к текущей версии страницы можно получить какCurrent и содержится отдельно от коллекции исторических версий.
type: docs
weight: 100
url: /ru/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Получает[`PageHistory`](../../pagehistory/) который содержит полную историю для каждой страницы, представленной в документе (самая ранняя с индексом 0). Доступ к текущей версии страницы можно получить как[`Current`](../../pagehistory/current/) и содержится отдельно от коллекции исторических версий.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| page | Page | Текущая версия страницы. |

### Возвращаемое значение

[`PageHistory`](../../pagehistory/) .

### Примеры

Показывает, как восстановить предыдущую версию страницы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Показывает, как редактировать историю страницы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


