---
title: Page
second_title: Справочник по API Aspose.Note для .NET
description: Представляет страницу.
type: docs
weight: 460
url: /ru/net/aspose.note/page/
---
## Page class

Представляет страницу.

```csharp
public sealed class Page : CompositeNode<IPageChildNode>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Page](page#constructor)() | Инициализирует новый экземпляр класса[`Page`](../page). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.note/page/author) { get; set; } | Получает или устанавливает автора. |
| [BackgroundColor](../../aspose.note/page/backgroundcolor) { get; set; } | Получает или устанавливает цвет фона страницы. |
| [CreationTime](../../aspose.note/page/creationtime) { get; set; } | Получает или задает время создания. |
| [Document](../../aspose.note/node/document) { get; } | Получает документ узла. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [IsConflictPage](../../aspose.note/page/isconflictpage) { get; set; } | Получает или задает значение, указывающее, является ли эта страница конфликтующей. |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/page/lastmodifiedtime) { get; set; } | Получает или задает время последнего изменения. |
| [Level](../../aspose.note/page/level) { get; set; } | Получает или устанавливает уровень. |
| [Margin](../../aspose.note/page/margin) { get; set; } | Получает или задает поле. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Получает следующий узел на том же уровне дерева узлов. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Получает тип узла. |
| [PageContentRevisionSummary](../../aspose.note/page/pagecontentrevisionsummary) { get; set; } | Получает или задает сводку изменений для страницы и ее дочерних узлов. |
| [PageLayoutSize](../../aspose.note/page/pagelayoutsize) { get; set; } | Получает или задает размер макета страницы, отображаемый в редакторе. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Получает родительский узел. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Получает предыдущий узел на том же уровне дерева узлов. |
| [SizeType](../../aspose.note/page/sizetype) { get; set; } | Получает или задает тип размера страницы. |
| [Title](../../aspose.note/page/title) { get; set; } | Получает или устанавливает заголовок. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Accept](../../aspose.note/page/accept)(DocumentVisitor) | Принимает посетителя узла. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [Clone](../../aspose.note/page/clone)(bool) | Клонирует страницу. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/page/getchildnodes#getchildnodes_1)() | Получить все дочерние узлы страницы по типу узла. |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IPageChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IPageChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

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

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
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
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Получить первую страницу
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Чтение сводки изменений содержимого для этой страницы
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Обновить сводку изменений страницы для этой страницы
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

// Загружаем изображение
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Вставляем изображение в узел документа
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Добавляем узел элемента контура
outline.AppendChildLast(outlineElem);

// Добавляем узел контура
page.AppendChildLast(outline);

// Добавляем узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // По умолчанию конфликтующие страницы просто пропускаются при сохранении.
    // Если отметить его как неконфликтный, то он будет сохранен как обычный в истории.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
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
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Создаем объект класса Document
Document doc = new Aspose.Note.Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Стиль по умолчанию для всего текста в документе.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Задаем свойства заголовка страницы
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Добавляем узел страницы в документ
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Инициализировать новый документ
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Инициализировать новую страницу
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Стиль по умолчанию для всего текста в документе.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Добавляем узел страницы
doc.AppendChildLast(page);

// Сохранение документа OneNote в разных форматах, установка размера шрифта текста и обнаружение изменений макета вручную.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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
string dataDir = RunExamples.GetDataDir_Pages();

// Создаем объект класса Document
Document doc = new Document();

// Инициализируем объект класса Page и устанавливаем его уровень
Aspose.Note.Page page1 = new Aspose.Note.Page(doc) { Level = 1 };

// Инициализируем объект класса Page и устанавливаем его уровень
Aspose.Note.Page page2 = new Aspose.Note.Page(doc) { Level = 2 };

// Инициализируем объект класса Page и устанавливаем его уровень
Aspose.Note.Page page3 = new Aspose.Note.Page(doc) { Level = 1 };

/*---------- Adding nodes to first Page ----------*/
Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "First page.", ParagraphStyle = textStyle };
outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page1.AppendChildLast(outline);

/*---------- Adding nodes to second Page ----------*/
var outline2 = new Outline(doc);
var outlineElem2 = new OutlineElement(doc);
var textStyle2 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text2 = new RichText(doc) { Text = "Second page.", ParagraphStyle = textStyle2 };
outlineElem2.AppendChildLast(text2);
outline2.AppendChildLast(outlineElem2);
page2.AppendChildLast(outline2);

/*---------- Adding nodes to third Page ----------*/
var outline3 = new Outline(doc);
var outlineElem3 = new OutlineElement(doc);
var textStyle3 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text3 = new RichText(doc) { Text = "Third page.", ParagraphStyle = textStyle3 };
outlineElem3.AppendChildLast(text3);
outline3.AppendChildLast(outlineElem3);
page3.AppendChildLast(outline3);

/*---------- Add pages to the OneNote Document ----------*/
doc.AppendChildLast(page1);
doc.AppendChildLast(page2);
doc.AppendChildLast(page3);

// Сохранить документ OneNote
dataDir = dataDir + "CreateDocWithRootAndSubPages_out.one";
doc.Save(dataDir);
```

Показывает, как получить метаинформацию о странице.

Показывает, как задать заголовок для страницы.

Показывает, как получить историю страницы.

Показывает, как редактировать метаинформацию страницы.

Показывает, как пройти по всем страницам и сделать замену в тексте.

Показывает, как пройтись по тексту страницы и произвести замену.

Показывает, как создать документ и сохранить его в формате html с параметрами по умолчанию.

Показывает, как добавить новое изображение с тегом.

Показывает, как проверить, является ли страница конфликтующей (т. е. имеет ли она изменения, которые OneNote не может автоматически объединить).

Показывает, как создать документ и сохранить в формате html указанный диапазон страниц.

Показывает, как создать документ с титульной страницей.

Показывает, как сохранить документ в разных форматах.

Показывает, как вставить новый список с китайской нумерацией.

Показывает, как вставить новый маркированный список.

Показывает, как вставить новый список с нумерацией.

Показывает, как добавить страницу с подстраницей.

### Смотрите также

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IPageChildNode](../ipagechildnode)
* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
