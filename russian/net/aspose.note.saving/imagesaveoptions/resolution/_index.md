---
title: ImageSaveOptions.Resolution
second_title: Справочник по API Aspose.Note для .NET
description: ImageSaveOptions свойство. Получает или задает разрешение сгенерированных изображений в точках на дюйм.
type: docs
weight: 50
url: /ru/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Получает или задает разрешение сгенерированных изображений в точках на дюйм.

```csharp
public float Resolution { get; set; }
```

### Примечания

Значение по умолчанию: 96.

### Примеры

Показывает, как установить разрешение изображения при сохранении документа как изображения.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Сохраняем документ.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Показывает, как сохранить записную книжку как изображение с указанными параметрами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

* class [ImageSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../imagesaveoptions/)
* сборка [Aspose.Note](../../../)


