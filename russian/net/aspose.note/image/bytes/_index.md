---
title: Image.Bytes
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает хранилище данных изображения.
type: docs
weight: 50
url: /ru/net/aspose.note/image/bytes/
---
## Image.Bytes property

Получает хранилище данных изображения.

```csharp
public byte[] Bytes { get; }
```

### Примеры

Показывает, как получить изображение из документа.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить все узлы изображения
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Сохраняем байты изображения в файл
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### Смотрите также

* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


