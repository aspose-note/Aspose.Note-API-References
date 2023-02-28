---
title: Interface INoteTag
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.INoteTag интерфейс. Интерфейс для тегов заметок т.е. тегов не связанных с задачами Outlook.
type: docs
weight: 180
url: /ru/net/aspose.note/inotetag/
---
## INoteTag interface

Интерфейс для тегов заметок (т.е. тегов, не связанных с задачами Outlook).

```csharp
public interface INoteTag : ITag
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Получает или задает цвет шрифта. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Получает или задает цвет выделения. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Получает или задает текст метки. |

### Примеры

Показывает, как получить доступ к сведениям о теге.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Получить все узлы RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Итерация по каждому узлу
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Получить свойства
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### Смотрите также

* interface [ITag](../itag/)
* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


