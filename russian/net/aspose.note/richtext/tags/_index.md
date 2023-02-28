---
title: RichText.Tags
second_title: Справочник по API Aspose.Note для .NET
description: RichText свойство. Получает список всех тегов абзаца.
type: docs
weight: 90
url: /ru/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Получает список всех тегов абзаца.

```csharp
public List<ITag> Tags { get; }
```

### Примеры

Показывает, как получить доступ к сведениям о задачах Outlook.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tasks();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить все узлы RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Итерация по каждому узлу
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Получить свойства
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Смотрите также

* interface [ITag](../../itag/)
* class [RichText](../)
* пространство имен [Aspose.Note](../../richtext/)
* сборка [Aspose.Note](../../../)


