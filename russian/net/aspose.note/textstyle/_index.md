---
title: Class TextStyle
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.TextStyle сорт. Определяет стиль текста.
type: docs
weight: 970
url: /ru/net/aspose.note/textstyle/
---
## TextStyle class

Определяет стиль текста.

```csharp
public sealed class TextStyle : Style
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TextStyle](textstyle/)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Получает стиль с культурой "en-US". |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Получает стиль по умолчанию для даты заголовка в MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Получает стиль по умолчанию для текста заголовка в MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Получает стиль по умолчанию для времени заголовка в MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Получает или задает цвет шрифта. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Получает или задает имя шрифта. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Получает или задает размер шрифта. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Получает стиль шрифта. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Получает или задает цвет выделения. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Получает или задает адрес гиперссылки. Должен быть установлен, если значение[`IsHyperlink`](./ishyperlink/) свойство истинно. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Получает или задает значение, указывающее, является ли текст полужирным. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Получает или задает значение, указывающее, скрыт ли стиль текста. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста гиперссылкой. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста курсивом. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста математическим форматированием. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста зачеркнутым. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста подстрочным. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста надстрочным. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста подчеркнутым. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Получает или задает язык текста. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Определяет, равен ли указанный объект текущему объекту. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Определяет, равен ли указанный объект текущему объекту. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Служит хэш-функцией для типа. |

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

Установите язык проверки для текста.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

Управляйте текстовым форматом, используя стиль абзаца.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

Показывает, как привязать гиперссылку к тексту.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tasks();

// Создаем объект класса Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Добавляем элементы контура
outline.AppendChildLast(outlineElem);

// Инициализировать объект класса Title
Title title = new Title() { TitleText = titleText };

// Инициализировать объект класса Page
Page page = new Note.Page() { Title = title };

// Добавляем узел Outline
page.AppendChildLast(outline);

// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Смотрите также

* class [Style](../style/)
* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


