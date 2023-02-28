---
title: ImageBinarizationOptions.BinarizationMethod
second_title: Справочник по API Aspose.Note для .NET
description: ImageBinarizationOptions свойство. Получает или задает метод бинаризации. Значение по умолчаниюFixedThreshold .
type: docs
weight: 20
url: /ru/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

Получает или задает метод бинаризации. Значение по умолчанию:FixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
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

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* пространство имен [Aspose.Note.Saving](../../imagebinarizationoptions/)
* сборка [Aspose.Note](../../../)


