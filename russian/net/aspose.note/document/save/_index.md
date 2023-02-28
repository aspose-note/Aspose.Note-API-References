---
title: Document.Save
second_title: Справочник по API Aspose.Note для .NET
description: Document метод. Сохраняет документ OneNote в файл.
type: docs
weight: 140
url: /ru/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Сохраняет документ OneNote в файл.

```csharp
public void Save(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл перезаписывается. |

### Исключения

| исключение | условие |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Структура документа нарушает спецификацию. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Запрошенный формат сохранения не поддерживается. |

### Примеры

Показывает, как сохранить документ.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Сохраняет документ OneNote в поток.

```csharp
public void Save(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | System.IO.Stream, в котором будет сохранен документ. |

### Исключения

| исключение | условие |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Структура документа нарушает спецификацию. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Запрошенный формат сохранения не поддерживается. |

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Сохраняет документ OneNote в файл в указанном формате.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл перезаписывается. |
| format | SaveFormat | Формат сохранения документа. |

### Исключения

| исключение | условие |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Структура документа нарушает спецификацию. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Запрошенный формат сохранения не поддерживается. |

### Примеры

Показывает, как сохранить документ с помощью перечисления SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Показывает, как сохранить документ в формате gif.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Сохраняем документ как gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### Смотрите также

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Сохраняет документ OneNote в поток в указанном формате.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | System.IO.Stream, в котором будет сохранен документ. |
| format | SaveFormat | Формат сохранения документа. |

### Исключения

| исключение | условие |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Структура документа нарушает спецификацию. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Запрошенный формат сохранения не поддерживается. |

### Примеры

Показывает, как сохранить документ в формате pdf с настройками по умолчанию.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Сохраняем документ как PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Показывает, как сохранить документ в поток.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Перемотать позицию потока обратно на ноль, чтобы она была готова для следующего чтения.
dstStream.Seek(0, SeekOrigin.Begin);
```

Показывает, как применить стиль темной темы к документу.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### Смотрите также

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Сохраняет документ OneNote в файл, используя указанные параметры сохранения.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл перезаписывается. |
| options | SaveOptions | Указывает параметры сохранения документа в файле. |

### Исключения

| исключение | условие |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Структура документа нарушает спецификацию. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Запрошенный формат сохранения не поддерживается. |

### Примеры

Показывает, как сохранить документ с помощью OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Показывает, как сохранить документ как изображение в формате Jpeg с помощью SaveFormat.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Сохраняем документ.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Показывает, как сохранить документ как изображение в формате Bmp с помощью ImageSaveOptions.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Сохраняем документ.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Показывает, как сохранить документ в формате Pdf с макетом страницы Letter.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Сохраняем документ.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Показывает, как сохранить документ в формате Pdf с макетом страницы A4 без ограничения высоты.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Сохраняем документ.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Показывает, как сохранить документ как изображение в градациях серого.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Сохраняем документ как gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Показывает, как сохранить документ как изображение в формате Tiff с использованием сжатия PackBits.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Сохраняем документ.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Показывает, как сохранить документ как изображение в формате Tiff с использованием сжатия Jpeg.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Сохраняем документ.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Показывает, как сохранить документ в виде изображения в формате Tiff с использованием сжатия факсов CCITT Group 3.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Сохраняем документ.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
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

Показывает, как сохранить документ в виде двоичного изображения с помощью метода Оцу.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Сохраняем документ как gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Показывает, как сохранить документ как бинарное изображение, используя фиксированный порог.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Сохраняем документ как gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### Смотрите также

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Сохраняет документ OneNote в поток, используя указанные параметры сохранения.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | System.IO.Stream, в котором будет сохранен документ. |
| options | SaveOptions | Указывает параметры сохранения документа в потоке. |

### Исключения

| исключение | условие |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Структура документа нарушает спецификацию. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Запрошенный формат сохранения не поддерживается. |

### Примеры

Показывает, как сохранить документ в формате pdf, используя указанный шрифт по умолчанию.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Сохраняем документ как PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Показывает, как сохранить документ в формате pdf, используя шрифт по умолчанию из файла.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Сохраняем документ как PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Показывает, как сохранить документ в формате pdf, используя шрифт по умолчанию из потока.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Сохраняем документ как PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Смотрите также

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


