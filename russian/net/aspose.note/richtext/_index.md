---
title: RichText
second_title: Справочник по API Aspose.Note для .NET
description: Представляет форматированный текст.
type: docs
weight: 510
url: /ru/net/aspose.note/richtext/
---
## RichText class

Представляет форматированный текст.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RichText](richtext#constructor)() | Инициализирует новый экземпляр класса[`RichText`](../richtext). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment) { get; set; } | Получает или задает выравнивание. |
| [Document](../../aspose.note/node/document) { get; } | Получает документ узла. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Получает значение, указывающее, является ли этот узел составным. Если true, узел может иметь дочерние узлы. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime) { get; set; } | Получает или задает время последнего изменения. |
| [Length](../../aspose.note/richtext/length) { get; } | Получает длину текста. |
| [LineSpacing](../../aspose.note/richtext/linespacing) { get; set; } | Получает или задает межстрочный интервал. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Получает следующий узел на том же уровне дерева узлов. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Получает тип узла. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle) { get; set; } | Получает или задает стиль абзаца. Эти настройки используются, если нет соответствующего объекта TextStyle в коллекцииStylesлибо этот объект не указывает необходимую настройку. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Получает родительский узел. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Получает предыдущий узел на том же уровне дерева узлов. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter) { get; set; } | Получает или устанавливает минимальное количество места после. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore) { get; set; } | Получает или задает минимальное количество места перед. |
| [Tags](../../aspose.note/richtext/tags) { get; } | Получает список всех тегов абзаца. |
| [Text](../../aspose.note/richtext/text) { get; set; } | Получает или задает текст. Строка НЕ ДОЛЖНА содержать символы со значением 10 (перевод строки). |
| [TextRuns](../../aspose.note/richtext/textruns) { get; } | Получает коллекцию текстов. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept)(DocumentVisitor) | Принимает посетителя узла. |
| [Append](../../aspose.note/richtext/append#append)(string) | Добавляет строку к последнему текстовому диапазону. |
| [Append](../../aspose.note/richtext/append#append_1)(string, TextStyle) | Добавляет строку в конец. |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront)(string) | Добавляет строку в начало первого текстового диапазона. |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront_1)(string, TextStyle) | Добавляет строку впереди. |
| [Clear](../../aspose.note/richtext/clear)() | Очищает содержимое этого экземпляра. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator)() | Возвращает перечислитель, перебирающий символы этого объекта RichText. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof)(char) | Возвращает отсчитываемый от нуля индекс первого вхождения указанного символа Unicode в этой строке. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_3)(string) | Возвращает отсчитываемый от нуля индекс первого вхождения указанной строки в данном экземпляре. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_1)(char, int) | Возвращает отсчитываемый от нуля индекс первого вхождения указанного символа Unicode в этой строке. Поиск начинается с указанной позиции символа. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_4)(string, int) | Возвращает отсчитываемый от нуля индекс первого вхождения указанной строки в данном экземпляре. Поиск начинается с указанной позиции символа. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_8)(string, StringComparison) | Возвращает отсчитываемый от нуля индекс первого вхождения указанной строки в текущем экземпляре. Параметр указывает тип поиска для указанной строки. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_2)(char, int, int) | Возвращает отсчитываемый от нуля индекс первого вхождения указанного символа в этом экземпляре. Поиск начинается с указанной позиции символа и проверяет указанное количество позиций символов. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_5)(string, int, int) | Возвращает отсчитываемый от нуля индекс первого вхождения указанной строки в данном экземпляре. Поиск начинается с указанной позиции символа и проверяет указанное количество позиций символов. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_7)(string, int, StringComparison) | Возвращает отсчитываемый от нуля индекс первого вхождения указанной строки в текущем экземпляре. Параметры определяют начальную позицию поиска в текущей строке и тип поиска для указанной строки. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_6)(string, int, int, StringComparison) | Возвращает отсчитываемый от нуля индекс первого вхождения указанной строки в текущем экземпляре. |
| [Insert](../../aspose.note/richtext/insert#insert)(int, string) | Вставляет указанную строку в указанную позицию индекса в этом экземпляре. |
| [Insert](../../aspose.note/richtext/insert#insert_1)(int, string, TextStyle) | Вставляет указанную строку с указанным стилем в указанную позицию индекса в этом экземпляре. |
| [Remove](../../aspose.note/richtext/remove#remove)(int) | Удаляет все символы в текущем экземпляре, начиная с указанной позиции и продолжая до последней позиции. |
| [Remove](../../aspose.note/richtext/remove#remove_1)(int, int) | Удаляет указанное количество символов в текущем экземпляре, начиная с указанной позиции. |
| [Replace](../../aspose.note/richtext/replace#replace)(char, char) | Заменяет все вхождения указанного символа Юникода в этом экземпляре другим указанным символом Юникода. |
| [Replace](../../aspose.note/richtext/replace#replace_1)(string, string) | Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой. |
| [Replace](../../aspose.note/richtext/replace#replace_2)(string, string, TextStyle) | Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой в указанном стиле. |
| [Trim](../../aspose.note/richtext/trim#trim)() | Удаляет все начальные и конечные пробельные символы. |
| [Trim](../../aspose.note/richtext/trim#trim_1)(char) | Удаляет все начальные и конечные экземпляры символа. |
| [Trim](../../aspose.note/richtext/trim#trim_2)(params char[]) | Удаляет все начальные и конечные вхождения набора символов, указанного в массиве. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend)() | Удаляет все конечные пробельные символы. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_1)(char) | Удаляет все вхождения символа в конце. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_2)(params char[]) | Удаляет все конечные вхождения набора символов, указанного в массиве. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart)() | Удаляет все начальные пробельные символы. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_1)(char) | Удаляет все начальные вхождения указанного символа. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_2)(params char[]) | Удаляет все ведущие вхождения набора символов, указанного в массиве. |

### Примеры

Показывает, как получить весь текст из документа.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить текст
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Печать текста на экране вывода
Console.WriteLine(text);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получаем список узлов страницы
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Получить текст
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Печать текста на экране вывода
    Console.WriteLine(text);
}
```

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
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Получаем список узлов таблицы
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Итерация по строкам таблицы
    foreach (TableRow row in table)
    {
        // Получить текст
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Печать текста на экране вывода
        Console.WriteLine(text);
    }
}
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Получаем список узлов таблицы
IList<Table> nodes = document.GetChildNodes<Table>();

// Установить количество таблиц
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Получить текст
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Печать текста на экране вывода
    Console.WriteLine(text);
}
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
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

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

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить все узлы RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Заменяем текст фигуры
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Сохраняем в любой поддерживаемый формат файла
oneFile.Save(dataDir, SaveFormat.Pdf);
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
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Получаем список узлов таблицы
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Итерация по строкам таблицы
    foreach (TableRow row in table)
    {
        // Получить список узлов TableCell
        // Итерация по ячейкам таблицы
        foreach (TableCell cell in row)
        {
            // Получить текст
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Печать текста на экране вывода
            Console.WriteLine(text);
        }
    }
}
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Получить все узлы RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Заменяем текст фигуры
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Сохраняем в любой поддерживаемый формат файла
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Инициализировать документ OneNote
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Стиль по умолчанию для всего текста в документе.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Сохраняем в формате HTML
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализировать объект класса OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Добавляем текстовый узел
outlineElem.AppendChildLast(text);

// Добавляем узел элемента контура
outline.AppendChildLast(outlineElem);

// Добавляем узел контура
page.AppendChildLast(outline);

// Добавляем узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Инициализировать документ OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Стиль по умолчанию для всего текста в документе.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Сохраняем в формате HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Получить все узлы RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Итерация по каждому узлу
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Получить свойства
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Page page = new Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализировать объект класса OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Инициализируем объект класса TextStyle и устанавливаем свойства форматирования
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Инициализировать объект класса RichText и применить стиль текста
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Добавляем узел RichText
outlineElem.AppendChildLast(text);

// Добавляем узел OutlineElement
outline.AppendChildLast(outlineElem);

// Добавляем узел Outline
page.AppendChildLast(outline);

// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Создаем объект класса Document
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
```

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

Показывает, как получить весь текст со страницы.

Выделим заголовки страниц среди других заголовков, увеличив размер шрифта.

Показывает, как получить текст из каждой строки таблицы.

Показывает, как получить текст из таблицы.

Подчеркнем последние изменения текста выделением.

Показывает, как задать заголовок для страницы.

Установить язык проверки для текста.

Показывает, как пройти по всем страницам и сделать замену в тексте.

Управление текстовым форматом с использованием стиля абзаца.

Показывает, как получить текст из ячеек таблицы.

Показывает, как пройтись по тексту страницы и произвести замену.

Показывает, как создать документ и сохранить его в формате html с параметрами по умолчанию.

Показывает, как добавить новый абзац с тегом.

Показывает, как создать документ и сохранить в формате html указанный диапазон страниц.

Показывает, как получить доступ к деталям тега.

Показывает, как создать документ с текстом.

Показывает, как вставить новый список с китайской нумерацией.

Показывает, как вставить новый маркированный список.

Показывает, как вставить новый список с нумерацией.

Показывает, как подготовить шаблон для еженедельной встречи.

Показывает, как привязать гиперссылку к тексту.

### Смотрите также

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [ITaggable](../itaggable)
* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
