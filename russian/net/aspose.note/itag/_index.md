---
title: ITag
second_title: Справочник по API Aspose.Note для .NET
description: Интерфейс для тегов всех видов.
type: docs
weight: 220
url: /ru/net/aspose.note/itag/
---
## ITag interface

Интерфейс для тегов всех видов.

```csharp
public interface ITag
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [CompletedTime](../../aspose.note/itag/completedtime) { get; set; } | Получает или задает завершенное время. |
| [CreationTime](../../aspose.note/itag/creationtime) { get; set; } | Получает или задает время создания. |
| [Icon](../../aspose.note/itag/icon) { get; set; } | Получает или задает значок. |
| [Label](../../aspose.note/itag/label) { get; } | Получает текст метки. |
| [Status](../../aspose.note/itag/status) { get; set; } | Получает или устанавливает статус. |

### Примеры

Показывает, как создать PDF-файл, содержащий все страницы, связанные с «Проектом А».

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

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

Показывает, как сделать заполненными все элементы флажков, связанные с «Проектом C».

Показывает, как открыть все элементы флажков, связанные с «Проектом C».

Показывает, как создать PDF-файл, содержащий страницы с элементами, отмеченными неполными флажками и созданными за последнюю неделю.

Показывает, как создать PDF-файл, содержащий страницы с незавершенными задачами Outlook, которые необходимо выполнить на этой неделе.

Показывает, как получить доступ к сведениям о задачах Outlook.

Показывает, как получить доступ к деталям тега.

### Смотрите также

* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
