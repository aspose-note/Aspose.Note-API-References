---
title: Enum FileFormat
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.FileFormat перечисление. Представляет формат файла OneNote.
type: docs
weight: 90
url: /ru/net/aspose.note/fileformat/
---
## FileFormat enumeration

Представляет формат файла OneNote.

```csharp
public enum FileFormat
```

### Ценности

| Имя | Ценность | Описание |
| --- | --- | --- |
| Unknown | `0` | Неизвестный формат файла. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote в Интернете. |

### Примеры

Показывает, как проверить, не произошла ли загрузка документа из-за того, что формат OneNote 2007 не поддерживается.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### Смотрите также

* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


