---
title: Style.IsBold
second_title: Справочник по API Aspose.Note для .NET
description: Style свойство. Получает или задает значение указывающее является ли текст полужирным.
type: docs
weight: 60
url: /ru/net/aspose.note/style/isbold/
---
## Style.IsBold property

Получает или задает значение, указывающее, является ли текст полужирным.

```csharp
public bool IsBold { get; set; }
```

### Примеры

Выделим заголовки страниц среди других заголовков, увеличив размер шрифта.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Перебираем заголовки страниц.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Подчеркнем последние изменения текста выделением.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Получить узлы RichText, измененные на прошлой неделе.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Установить цвет выделения
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Установить цвет выделения
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Смотрите также

* class [Style](../)
* пространство имен [Aspose.Note](../../style/)
* сборка [Aspose.Note](../../../)


