---
title: Notebook.DisplayName
second_title: Справочник по API Aspose.Note для .NET
description: Notebook свойство. Получает или задает отображаемое имя.
type: docs
weight: 40
url: /ru/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Получает или задает отображаемое имя.

```csharp
public string DisplayName { get; set; }
```

### Примеры

Показывает, как удалить раздел из блокнота.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Проходим через его дочерние узлы для поиска нужного дочернего элемента
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Удалить дочерний элемент из блокнота
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Сохраняем блокнот
notebook.Save(dataDir);
```

### Смотрите также

* class [Notebook](../)
* пространство имен [Aspose.Note](../../notebook/)
* сборка [Aspose.Note](../../../)


