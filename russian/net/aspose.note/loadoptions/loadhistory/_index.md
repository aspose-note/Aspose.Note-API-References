---
title: LoadOptions.LoadHistory
second_title: Справочник по API Aspose.Note для .NET
description: LoadOptions свойство. Получает или задает значение указывающее должен ли загрузчик документов игнорировать историю. Используйте этот параметр чтобы уменьшить использование памяти и ЦП. Значение по умолчаниюистинный .
type: docs
weight: 30
url: /ru/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Получает или задает значение, указывающее, должен ли загрузчик документов игнорировать историю. Используйте этот параметр, чтобы уменьшить использование памяти и ЦП. Значение по умолчанию:`истинный` .

```csharp
public bool LoadHistory { get; set; }
```

### Примеры

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

* class [LoadOptions](../)
* пространство имен [Aspose.Note](../../loadoptions/)
* сборка [Aspose.Note](../../../)


