---
title: Enum BinarizationMethod
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Saving.BinarizationMethod 枚举. 指定图像的二值化方法
type: docs
weight: 560
url: /zh/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

指定图像的二值化方法。

```csharp
public enum BinarizationMethod
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| FixedThreshold | `0` | 使用指定的固定阈值执行图像的二值化。 |
| Otsu | `1` | 图像的二值化是使用 Otsu 的方法自适应执行的，以评估阈值。 |

### 例子

展示如何使用 Otsu 的方法将文档保存为二进制图像。

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

显示如何使用固定阈值将文档保存为二值图像。

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

### 也可以看看

* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving/)
* 部件 [Aspose.Note](../../)


