---
title: "枚举 BinarizationMethod"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.BinarizationMethod 枚举。指定图像的二值化方法"
type: docs
weight: 640
url: /zh/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

指定图像的二值化方法。

```csharp
public enum BinarizationMethod
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| FixedThreshold | `0` | 图像的二值化使用指定的固定阈值进行。 |
| Otsu | `1` | 图像的二值化采用自适应方式，使用大津法评估阈值。 |

## 示例

展示如何使用 Otsu 方法将文档保存为二值图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// 将文档保存为 gif。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

展示如何使用固定阈值将文档保存为二值图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// 将文档保存为 gif。
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

### 另请参阅

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


