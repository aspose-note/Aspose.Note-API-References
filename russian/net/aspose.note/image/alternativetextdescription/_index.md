---
title: Image.AlternativeTextDescription
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает или задает текст альтернативного текста для изображения.
type: docs
weight: 30
url: /ru/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

Получает или задает текст альтернативного текста для изображения.

```csharp
public string AlternativeTextDescription { get; set; }
```

### Примеры

Показывает, как установить текстовое описание для изображения.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

### Смотрите также

* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


