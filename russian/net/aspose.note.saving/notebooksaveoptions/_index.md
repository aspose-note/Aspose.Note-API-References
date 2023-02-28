---
title: Class NotebookSaveOptions
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.NotebookSaveOptions сорт. Абстрактный базовый класс представляющий параметры сохранения записной книжки для определенного формата.
type: docs
weight: 790
url: /ru/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

Абстрактный базовый класс, представляющий параметры сохранения записной книжки для определенного формата.

```csharp
public abstract class NotebookSaveOptions
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Получает или задает значение, указывающее, следует ли сохранять дочерние документы явно. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Получает или задает значение, указывающее, сохраняется ли иерархия дочерних элементов записной книжки в свернутом виде. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Получает формат, в котором сохранена записная книжка. |

## Методы

| Имя | Описание |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Получает параметры сохранения для всех дочерних документов записной книжки. |

### Примеры

Показывает, как сохранить плоский блокнот в формате pdf.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Сохраняем блокнот
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

Показывает, как сохранить плоский блокнот как изображение.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
```

### Смотрите также

* пространство имен [Aspose.Note.Saving](../../aspose.note.saving/)
* сборка [Aspose.Note](../../)


