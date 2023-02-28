---
title: PageSettings.A4NoHeightLimit
second_title: Справочник по API Aspose.Note для .NET
description: PageSettings свойство. Получает настройки для страницы формата A4 с неограниченной высотой.
type: docs
weight: 20
url: /ru/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Получает настройки для страницы формата A4 с неограниченной высотой.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Примеры

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

* class [PageSettings](../)
* пространство имен [Aspose.Note.Saving](../../pagesettings/)
* сборка [Aspose.Note](../../../)


