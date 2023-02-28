---
title: PdfSaveOptions.PageSettings
second_title: Справочник по API Aspose.Note для .NET
description: PdfSaveOptions свойство. Получает или задает параметры страницы для каждой страницы в документе. По умолчанию зависит от CurrentUICulture.
type: docs
weight: 40
url: /ru/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Получает или задает параметры страницы для каждой страницы в документе. По умолчанию зависит от CurrentUICulture.

```csharp
public PageSettings PageSettings { get; set; }
```

### Примеры

Показывает, как сохранить документ в формате Pdf с макетом страницы Letter.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Сохраняем документ.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Показывает, как сохранить документ в формате Pdf с макетом страницы A4 без ограничения высоты.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Сохраняем документ.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Смотрите также

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../pdfsaveoptions/)
* сборка [Aspose.Note](../../../)


