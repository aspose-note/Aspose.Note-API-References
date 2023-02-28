---
title: ImageSaveOptions.BinarizationOptions
second_title: Справочник по API Aspose.Note для .NET
description: ImageSaveOptions свойство. Получает или задает параметры бинаризации изображения.
type: docs
weight: 20
url: /ru/net/aspose.note.saving/imagesaveoptions/binarizationoptions/
---
## ImageSaveOptions.BinarizationOptions property

Получает или задает параметры бинаризации изображения.

```csharp
public ImageBinarizationOptions BinarizationOptions { get; set; }
```

### Примеры

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

* class [ImageBinarizationOptions](../../imagebinarizationoptions/)
* class [ImageSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../imagesaveoptions/)
* сборка [Aspose.Note](../../../)


