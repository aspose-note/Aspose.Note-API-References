---
title: Image.HyperlinkUrl
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает или задает гиперссылку связанную с изображением.
type: docs
weight: 110
url: /ru/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Получает или задает гиперссылку, связанную с изображением.

```csharp
public string HyperlinkUrl { get; set; }
```

### Примеры

Показывает, как привязать гиперссылку к изображению.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### Смотрите также

* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


