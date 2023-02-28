---
title: PageSettings.Letter
second_title: Справочник по API Aspose.Note для .NET
description: PageSettings свойство. Получает настройки для страницы формата Letter.
type: docs
weight: 30
url: /ru/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Получает настройки для страницы формата Letter.

```csharp
public static PageSettings Letter { get; }
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

### Смотрите также

* class [PageSettings](../)
* пространство имен [Aspose.Note.Saving](../../pagesettings/)
* сборка [Aspose.Note](../../../)


