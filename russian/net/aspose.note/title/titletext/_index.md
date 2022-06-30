---
title: TitleText
second_title: Справочник по API Aspose.Note для .NET
description: Получает или задает текст заголовка.
type: docs
weight: 60
url: /ru/net/aspose.note/title/titletext/
---
## Title.TitleText property

Получает или задает текст заголовка.

```csharp
public RichText TitleText { get; set; }
```

### Примеры

Показывает, как редактировать историю страницы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
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

Показывает, как задать заголовок для страницы.

Показывает, как создать документ и сохранить его в формате html с параметрами по умолчанию.

Показывает, как создать документ и сохранить в формате html указанный диапазон страниц.

Показывает, как создать документ с титульной страницей.

Показывает, как сохранить документ в разных форматах.

### Смотрите также

* class [RichText](../../richtext)
* class [Title](../../title)
* пространство имен [Aspose.Note](../../title)
* сборка [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
