---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Справочник по API Aspose.Note для .NET
description: NotebookSaveOptions свойство. Получает или задает параметры сохранения для всех дочерних документов записной книжки.
type: docs
weight: 10
url: /ru/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Получает или задает параметры сохранения для всех дочерних документов записной книжки.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### Примеры

Показывает, как сохранить блокнот в формате pdf с указанными параметрами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
```

### Смотрите также

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* пространство имен [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* сборка [Aspose.Note](../../../)


