---
title: Notebook.RemoveChild
second_title: Справочник по API Aspose.Note для .NET
description: Notebook метод. Удаляет дочерний узел.
type: docs
weight: 140
url: /ru/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

Удаляет дочерний узел.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| oldChild | INotebookChildNode | Удаляемый узел. |

### Возвращаемое значение

Удаленный узел.

### Примеры

Показывает, как получить доступ ко всем разделам из записной книжки.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
```

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

Показывает, как сохранить блокнот.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### Смотрите также

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* пространство имен [Aspose.Note](../../notebook/)
* сборка [Aspose.Note](../../../)


