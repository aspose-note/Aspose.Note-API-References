---
title: SaveFormat
second_title: Справочник по API Aspose.Note для .NET
description: Указывает формат в котором сохранен документ.
type: docs
weight: 520
url: /ru/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Указывает формат, в котором сохранен документ.

```csharp
public enum SaveFormat
```

### Ценности

| Имя | Ценность | Описание |
| --- | --- | --- |
| Png | `1` | Указывает, что выходным файлом является PNG-файл. |
| Bmp | `2` | Указывает, что выходным файлом является файл BMP. |
| Jpeg | `3` | Указывает, что выходным файлом является файл JPEG. |
| Gif | `4` | Указывает, что выходным файлом является файл GIF. |
| Tiff | `5` | Указывает, что выходным файлом является файл TIFF. |
| Pdf | `6` | Указывает, что выходным файлом является PDF-файл. |
| One | `7` | Указывает, что выходным файлом является файл OneNote. |
| Html | `8` | Указывает, что результатом является HTML-файл. |

### Примеры

Показывает, как сохранить документ с помощью перечисления SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Сохраняем документ как PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Сохраняем документ.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Сохраняем документ как gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Сохраняем документ.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Сохраняем документ.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Сохраняем документ.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

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

Показывает, как сохранить документ в формате pdf с настройками по умолчанию.

Показывает, как сохранить документ как изображение в формате Jpeg с помощью SaveFormat.

Показывает, как сохранить документ в формате gif.

Показывает, как установить качество изображения при сохранении документа как изображения в формате JPEG.

Показывает, как сохранить документ как изображение в формате Bmp с помощью ImageSaveOptions.

Показывает, как установить разрешение изображения при сохранении документа как изображения.

Показывает, как сохранить документ как изображение в градациях серого.

Показывает, как сохранить документ в виде изображения в формате Tiff с использованием сжатия PackBits.

Показывает, как сохранить документ как изображение в формате Tiff с использованием сжатия Jpeg.

Показывает, как сохранить документ в виде изображения в формате Tiff с использованием сжатия факсов CCITT Group 3.

Показывает, как сохранить документ в виде двоичного изображения с помощью метода Оцу.

Показывает, как сохранить документ как бинарное изображение с использованием фиксированного порога.

### Смотрите также

* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
