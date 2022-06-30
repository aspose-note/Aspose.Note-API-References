---
title: PdfSaveOptions
second_title: Справочник по API Aspose.Note для .NET
description: Позволяет указать дополнительные параметры при рендеринге страниц документа в PDF.
type: docs
weight: 820
url: /ru/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Позволяет указать дополнительные параметры при рендеринге страниц документа в PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Получает или задает настройки шрифта, которые будут использоваться при сохранении |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | Получает или задает тип сжатия, применяемый к изображениям в файле PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | Получает или задает значение, определяющее качество изображений JPEG внутри документа PDF. Значение может варьироваться от 0 до 100, где 0 означает худшее качество, но максимальное сжатие, а 100 означает лучшее качество, но минимальное сжатие. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Получает или задает количество сохраняемых страниц. По умолчанию этоMaxValue что означает, что будут отображаться все страницы документа. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Получает или задает индекс первой страницы для сохранения. По умолчанию 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | Получает или задает алгоритм, используемый для разделения страниц. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Получает формат, в котором сохранен документ. |

### Примеры

Показывает, как сохранить блокнот в формате pdf с указанными параметрами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// или же
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

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

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Или же
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Или же
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Или же
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Или же
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

Когда длинные страницы OneNote сохраняются в формате pdf, они разбиваются на страницы. В примере показано, как настроить логику разделения объектов, расположенных на разрывах страниц.

Показывает, как сохранить документ в формате pdf.

Показывает, как сохранить документ в формате pdf, используя определенные настройки.

Когда длинные страницы OneNote сохраняются в формате pdf, они разбиваются на страницы. В примере показано, как настроить логику разделения объектов, расположенных на разрывах страниц.

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Note.Saving](../../aspose.note.saving)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
