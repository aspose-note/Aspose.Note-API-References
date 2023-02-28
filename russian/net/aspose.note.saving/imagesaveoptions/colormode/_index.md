---
title: ImageSaveOptions.ColorMode
second_title: Справочник по API Aspose.Note для .NET
description: ImageSaveOptions свойство. Получает или устанавливаетColorMode для выходного изображения.
type: docs
weight: 30
url: /ru/net/aspose.note.saving/imagesaveoptions/colormode/
---
## ImageSaveOptions.ColorMode property

Получает или устанавливает`ColorMode` для выходного изображения.

```csharp
public ColorMode ColorMode { get; set; }
```

### Примеры

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

* enum [ColorMode](../../colormode/)
* class [ImageSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../imagesaveoptions/)
* сборка [Aspose.Note](../../../)


