---
title: Class HtmlSaveOptions
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.HtmlSaveOptions сорт. Позволяет указать дополнительные параметры при сохранении документа в формате HTML.
type: docs
weight: 700
url: /ru/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Позволяет указать дополнительные параметры при сохранении документа в формате HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Получает или задает, будет ли файл таблицы стилей создаваться для каждой новой страницы отдельно. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Получает или задает значение, указывающее, включено ли создание документа на странице. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Получает или задает способ экспорта css. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Получает или задает способ экспорта шрифтов. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Получает или задает способ экспорта изображений. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Получает или задает типы шрифта. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения шрифта. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Получает или задает настройки шрифта, которые будут использоваться при сохранении |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения изображения. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Получает или задает количество сохраняемых страниц. По умолчаниюMaxValue означает, что будут отображены все страницы документа. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Получает или задает индекс первой страницы для сохранения. По умолчанию 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения страницы. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Получает формат, в котором сохранен документ. |

### Примеры

Показывает, как сохранить документ в формате html с сохранением всех ресурсов (css/шрифты/изображения) в отдельные файлы.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Показывает, как сохранить документ в поток в формате html с встраиванием всех ресурсов (css/шрифты/изображения).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
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

Показывает, как сохранить документ в формате html с сохранением всех ресурсов (css/шрифты/изображения) с помощью пользовательских обратных вызовов.

```csharp
// Код ниже создает папку «documentFolder», содержащую document.html, папку «css» с файлом «style.css», папку «images» с изображениями и папку «fonts» со шрифтами.
// Файл 'style.css' будет содержать в конце следующую строку "/* Эта строка добавляется к потоку вручную пользователем */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Смотрите также

* class [SaveOptions](../saveoptions/)
* пространство имен [Aspose.Note.Saving](../../aspose.note.saving/)
* сборка [Aspose.Note](../../)


