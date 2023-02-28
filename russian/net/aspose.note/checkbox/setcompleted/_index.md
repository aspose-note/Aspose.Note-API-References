---
title: CheckBox.SetCompleted
second_title: Справочник по API Aspose.Note для .NET
description: CheckBox метод. Устанавливает тег в завершенное состояние.
type: docs
weight: 70
url: /ru/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Устанавливает тег в завершенное состояние.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| completedTime | DateTime | Завершенное время. |

### Смотрите также

* class [CheckBox](../)
* пространство имен [Aspose.Note](../../checkbox/)
* сборка [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Устанавливает тег в завершенное состояние, используя текущее время как завершенное время.

```csharp
public void SetCompleted()
```

### Примеры

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

### Смотрите также

* class [CheckBox](../)
* пространство имен [Aspose.Note](../../checkbox/)
* сборка [Aspose.Note](../../../)


