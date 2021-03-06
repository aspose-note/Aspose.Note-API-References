---
title: AlternativeTextTitle
second_title: Справочник по API Aspose.Note для .NET
description: Получает или задает заголовок альтернативного текста для изображения.
type: docs
weight: 40
url: /ru/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Получает или задает заголовок альтернативного текста для изображения.

```csharp
public string AlternativeTextTitle { get; set; }
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

* class [Image](../../image)
* пространство имен [Aspose.Note](../../image)
* сборка [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
