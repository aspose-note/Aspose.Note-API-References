---
title: UnsupportedFileFormatException.FileFormat
second_title: Справочник по API Aspose.Note для .NET
description: UnsupportedFileFormatException свойство. Получает формат файла переданных данных если обнаружен.
type: docs
weight: 10
url: /ru/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Получает формат файла переданных данных, если обнаружен.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* пространство имен [Aspose.Note](../../unsupportedfileformatexception/)
* сборка [Aspose.Note](../../../)


