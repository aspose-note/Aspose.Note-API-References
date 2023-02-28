---
title: Image.OriginalWidth
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает исходную ширину. Это исходная ширина изображения до изменения размера.
type: docs
weight: 150
url: /ru/net/aspose.note/image/originalwidth/
---
## Image.OriginalWidth property

Получает исходную ширину. Это исходная ширина изображения до изменения размера.

```csharp
public float OriginalWidth { get; }
```

### Примеры

Показывает, как получить метаинформацию изображения.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить все узлы изображения
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

### Смотрите также

* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


