---
title: Page.BackgroundColor
second_title: Справочник по API Aspose.Note для .NET
description: Page свойство. Получает или устанавливает цвет фона страницы.
type: docs
weight: 30
url: /ru/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Получает или устанавливает цвет фона страницы.

```csharp
public Color BackgroundColor { get; set; }
```

### Примеры

Показывает, как установить цвет фона страницы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Показывает, как применить стиль темной темы к документу.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### Смотрите также

* class [Page](../)
* пространство имен [Aspose.Note](../../page/)
* сборка [Aspose.Note](../../../)


