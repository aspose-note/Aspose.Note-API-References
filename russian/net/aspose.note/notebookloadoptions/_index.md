---
title: Class NotebookLoadOptions
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.NotebookLoadOptions сорт. Параметры используемые для загрузки блокнота.
type: docs
weight: 420
url: /ru/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Параметры, используемые для загрузки блокнота.

```csharp
public class NotebookLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Получает или задает значение, указывающее, следует ли явно загружать дочерние документы позже. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Получает или задает значение, указывающее, следует ли загружать дочерние документы во время загрузки родительского документа. |

### Примеры

Показывает, как зашифровать блокнот.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Смотрите также

* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


