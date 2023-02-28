---
title: Class ImageSaveOptions
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.ImageSaveOptions сорт. Позволяет указать дополнительные параметры при преобразовании страниц документа в изображения.
type: docs
weight: 720
url: /ru/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Позволяет указать дополнительные параметры при преобразовании страниц документа в изображения.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Инициализирует новый экземпляр`ImageSaveOptions` класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Получает или задает параметры бинаризации изображения. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Получает или устанавливает[`ColorMode`](./colormode/) для выходного изображения. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Получает или задает настройки шрифта, которые будут использоваться при сохранении |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Получает или задает количество сохраняемых страниц. По умолчаниюMaxValue означает, что будут отображены все страницы документа. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Получает или задает индекс первой страницы для сохранения. По умолчанию 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Получает или задает значение, определяющее качество сохраненного изображения. Это значение передается кодеку как параметр System.Drawing.Imaging.Encoder.Quality. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Получает или задает разрешение сгенерированных изображений в точках на дюйм. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Получает формат, в котором сохранен документ. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Получает или задает тип сжатия для использования при сохранении сгенерированных изображений в формате TIFF. |

### Примеры

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

Показывает, как установить качество изображения при сохранении документа как изображения в формате JPEG.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Сохраняем документ.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
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

Показывает, как установить разрешение изображения при сохранении документа как изображения.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Сохраняем документ.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
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

Показывает, как сохранить записную книжку как изображение с указанными параметрами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
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

Показывает, как сохранить плоский блокнот как изображение.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
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

* class [SaveOptions](../saveoptions/)
* пространство имен [Aspose.Note.Saving](../../aspose.note.saving/)
* сборка [Aspose.Note](../../)


