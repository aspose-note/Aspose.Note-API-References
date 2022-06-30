---
title: Text
second_title: Справочник по API Aspose.Note для .NET
description: Получает или задает текст. Строка НЕ ДОЛЖНА содержать символы со значением 10 перевод строки.
type: docs
weight: 100
url: /ru/net/aspose.note/richtext/text/
---
## RichText.Text property

Получает или задает текст. Строка НЕ ДОЛЖНА содержать символы со значением 10 (перевод строки).

```csharp
public string Text { get; set; }
```

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

Показывает, как получить текст из каждой строки таблицы.

Показывает, как получить текст из таблицы.

Показывает, как задать заголовок для страницы.

Показывает, как пройти по всем страницам и сделать замену в тексте.

Показывает, как получить текст из ячеек таблицы.

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

* class [RichText](../../richtext)
* пространство имен [Aspose.Note](../../richtext)
* сборка [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
