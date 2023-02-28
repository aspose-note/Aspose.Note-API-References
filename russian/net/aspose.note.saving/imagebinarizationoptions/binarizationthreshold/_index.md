---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Справочник по API Aspose.Note для .NET
description: ImageBinarizationOptions свойство. Получает или задает пороговое значение для метода бинаризации с фиксированным порогом. Значение по умолчанию 128.
type: docs
weight: 30
url: /ru/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Получает или задает пороговое значение для метода бинаризации с фиксированным порогом. Значение по умолчанию: 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Примеры

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

* class [ImageBinarizationOptions](../)
* пространство имен [Aspose.Note.Saving](../../imagebinarizationoptions/)
* сборка [Aspose.Note](../../../)


