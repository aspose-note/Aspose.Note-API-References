---
title: ParagraphStyle
second_title: Справочник по API Aspose.Note для .NET
description: Настройки стиля текста которые будут использоваться если нет соответствующего объекта TextStyle в коллекцииStylesлибо этот объект не указывает необходимый параметр.
type: docs
weight: 490
url: /ru/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Настройки стиля текста, которые будут использоваться, если нет соответствующего объекта TextStyle в коллекцииStylesлибо этот объект не указывает необходимый параметр.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ParagraphStyle](paragraphstyle)() | Инициализирует новый экземпляр класса[`ParagraphStyle`](../paragraphstyle). |

## Характеристики

| Имя | Описание |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default) { get; } | Получает ParagraphStyle с настройками по умолчанию. |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | Получает или задает цвет шрифта. |
| [FontName](../../aspose.note/style/fontname) { get; set; } | Получает или задает имя шрифта. |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | Получает или задает размер шрифта. |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | Получает стиль шрифта. |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | Получает или задает цвет выделения. |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста полужирным. |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста курсивом. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста зачеркнутым. |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста индексом. |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста надстрочным. |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста подчеркнутым. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals#equals_1)(object) | Определяет, равен ли указанный объект текущему объекту. |
| [Equals](../../aspose.note/paragraphstyle/equals#equals)(ParagraphStyle) | Определяет, равен ли указанный объект текущему объекту. |
| override [GetHashCode](../../aspose.note/style/gethashcode)() | Служит хэш-функцией для типа. |

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

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Инициализировать документ OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Инициализировать страницу OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Применяем настройки стиля текста
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Числа в одном контуре автоматически увеличиваются.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------------------------------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------------------------------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------------------------------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Создаем объект класса Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализируем объект класса TextStyle и устанавливаем свойства форматирования
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Инициализируем объекты класса OutlineElement и применяем маркеры
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Инициализировать объект класса RichText и применить стиль текста
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Добавляем элементы контура
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Добавляем узел Outline
page.AppendChildLast(outline);
// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализируем объект класса TextStyle и устанавливаем свойства форматирования
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Инициализировать объекты класса OutlineElement и применить нумерацию
// Числа в одном контуре автоматически увеличиваются.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Добавляем элементы контура
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Добавляем узел Outline
page.AppendChildLast(outline);

// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

Подчеркнем последние изменения текста выделением.

Управление текстовым форматом с использованием стиля абзаца.

Показывает, как вставить новый список с китайской нумерацией.

Показывает, как вставить новый маркированный список.

Показывает, как вставить новый список с нумерацией.

### Смотрите также

* class [Style](../style)
* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
