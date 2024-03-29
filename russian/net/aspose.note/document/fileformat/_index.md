---
title: Document.FileFormat
second_title: Справочник по API Aspose.Note для .NET
description: Document свойство. Получает формат файла OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /ru/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Получает формат файла (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Примеры

Показывает, как получить формат файла документа.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Обработка OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Обработка OneNote в сети
        break;
}
```

### Смотрите также

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


