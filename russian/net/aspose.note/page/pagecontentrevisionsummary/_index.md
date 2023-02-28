---
title: Page.PageContentRevisionSummary
second_title: Справочник по API Aspose.Note для .NET
description: Page свойство. Получает или задает сводку изменений для страницы и ее дочерних узлов.
type: docs
weight: 90
url: /ru/net/aspose.note/page/pagecontentrevisionsummary/
---
## Page.PageContentRevisionSummary property

Получает или задает сводку изменений для страницы и ее дочерних узлов.

```csharp
public RevisionSummary PageContentRevisionSummary { get; set; }
```

### Примеры

Показывает, как редактировать метаинформацию страницы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Чтение сводки изменений содержимого для этой страницы
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Обновить сводку изменений страницы для этой страницы
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

* class [RevisionSummary](../../revisionsummary/)
* class [Page](../)
* пространство имен [Aspose.Note](../../page/)
* сборка [Aspose.Note](../../../)


