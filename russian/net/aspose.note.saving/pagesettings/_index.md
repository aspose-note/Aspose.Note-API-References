---
title: Class PageSettings
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.PageSettings сорт. Представляет параметры макета страницы.
type: docs
weight: 820
url: /ru/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Представляет параметры макета страницы.

```csharp
public class PageSettings
```

## Характеристики

| Имя | Описание |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Получает настройки для страницы формата A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Получает настройки для страницы формата A4 с неограниченной высотой. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Получает настройки для страницы формата Letter. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Получает настройки для страницы формата Letter с неограниченной высотой. |

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

* пространство имен [Aspose.Note.Saving](../../aspose.note.saving/)
* сборка [Aspose.Note](../../)


