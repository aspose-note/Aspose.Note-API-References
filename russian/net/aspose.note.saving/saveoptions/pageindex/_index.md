---
title: SaveOptions.PageIndex
second_title: Справочник по API Aspose.Note для .NET
description: SaveOptions свойство. Получает или задает индекс первой страницы для сохранения. По умолчанию 0.
type: docs
weight: 30
url: /ru/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Получает или задает индекс первой страницы для сохранения. По умолчанию 0.

```csharp
public int PageIndex { get; set; }
```

### Примеры

Показывает, как сохранить документ в формате png.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Инициализировать объект ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Установить индекс страницы
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Сохраняем документ в формате PNG.
oneFile.Save(dataDir, opts);
```

Показывает, как сохранить документ в формате pdf.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Инициализировать объект PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Установить индекс первой страницы для сохранения
                              PageIndex = 0,

                              // Установить количество страниц
                              PageCount = 1,
                          };

// Сохраняем документ как PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Показывает, как сохранить документ в формате pdf, используя определенные настройки.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Инициализировать объект PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Использовать сжатие JPEG
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Качество сжатия JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Показывает, как создать документ и сохранить в формате html заданный диапазон страниц.

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

Показывает, как создать документ с форматированным форматированным текстом.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Page page = new Page();

// Инициализировать объект класса Title
Title title = new Title();

// Инициализируем объект класса TextStyle и устанавливаем свойства форматирования
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// Установить заголовок страницы
page.Title = title;

// Добавляем узел RichText
outlineElem.AppendChildLast(text);

// Добавляем узел OutlineElement
outline.AppendChildLast(outlineElem);

// Добавляем узел Outline
page.AppendChildLast(outline);

// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Смотрите также

* class [SaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../saveoptions/)
* сборка [Aspose.Note](../../../)


