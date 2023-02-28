---
title: AttachedFile.Bytes
second_title: Справочник по API Aspose.Note для .NET
description: AttachedFile свойство. Получает двоичные данные для внедренного файла.
type: docs
weight: 50
url: /ru/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Получает двоичные данные для внедренного файла.

```csharp
public byte[] Bytes { get; }
```

### Примеры

Показывает, как получить содержимое вложенного файла.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Attachments();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Получаем список узлов прикрепленных файлов
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Перебираем все узлы
foreach (AttachedFile file in nodes)
{
    // Загружаем прикрепленный файл в объект потока
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Создаем локальный файл
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Копируем файловый поток
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Смотрите также

* class [AttachedFile](../)
* пространство имен [Aspose.Note](../../attachedfile/)
* сборка [Aspose.Note](../../../)


