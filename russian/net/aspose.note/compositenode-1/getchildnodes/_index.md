---
title: CompositeNode1.GetChildNodes
second_title: Справочник по API Aspose.Note для .NET
description: CompositeNode метод. Получить все дочерние узлы по типу узла.
type: docs
weight: 70
url: /ru/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Получить все дочерние узлы по типу узла.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Параметр | Описание |
| --- | --- |
| T1 | Тип элементов в возвращаемом списке. |

### Возвращаемое значение

Список дочерних узлов.

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* пространство имен [Aspose.Note](../../compositenode-1/)
* сборка [Aspose.Note](../../../)


