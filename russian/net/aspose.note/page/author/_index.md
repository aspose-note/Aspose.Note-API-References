---
title: Page.Author
second_title: Справочник по API Aspose.Note для .NET
description: Page свойство. Получает или задает автора.
type: docs
weight: 20
url: /ru/net/aspose.note/page/author/
---
## Page.Author property

Получает или задает автора.

```csharp
public string Author { get; set; }
```

### Примеры

Показывает, как получить метаинформацию о странице.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Показывает, как получить историю страницы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Получить первую страницу
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Смотрите также

* class [Page](../)
* пространство имен [Aspose.Note](../../page/)
* сборка [Aspose.Note](../../../)


