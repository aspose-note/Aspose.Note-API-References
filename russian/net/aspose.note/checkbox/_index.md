---
title: Class CheckBox
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.CheckBox сорт. Базовый класс для тегов которые могут переключать свое состояние между полным и незавершенным.
type: docs
weight: 20
url: /ru/net/aspose.note/checkbox/
---
## CheckBox class

Базовый класс для тегов, которые могут переключать свое состояние между полным и незавершенным.

```csharp
public abstract class CheckBox : ITag
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Получает значение, указывающее, находится ли CheckBox в проверенном состоянии. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Получает или устанавливает завершенное время. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Получает или задает время создания. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Получает или задает значок. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Получает текст метки. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Получает или устанавливает статус. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Устанавливает тег в завершенное состояние, используя текущее время как завершенное время. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Устанавливает тег в завершенное состояние. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Устанавливает тег в открытое состояние. |

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

Показывает, как сделать заполненными все элементы флажков, связанные с «Проектом C».

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

Показывает, как открыть все элементы флажка, связанные с «Проектом C».

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

Показывает, как создать PDF-файл, содержащий страницы с элементами, отмеченными незавершенными флажками и созданными за последнюю неделю.

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

Показывает, как создать PDF-файл, содержащий страницы с незавершенными задачами Outlook, которые необходимо выполнить на этой неделе.

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

### Смотрите также

* interface [ITag](../itag/)
* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


