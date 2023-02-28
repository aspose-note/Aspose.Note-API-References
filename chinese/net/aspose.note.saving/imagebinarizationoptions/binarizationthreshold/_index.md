---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note for .NET API 参考
description: ImageBinarizationOptions 财产. 获取或设置固定阈值二值化方法的阈值 默认值为 128.
type: docs
weight: 30
url: /zh/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

获取或设置固定阈值二值化方法的阈值。 默认值为 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### 例子

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

* class [ImageBinarizationOptions](../)
* 命名空间 [Aspose.Note.Saving](../../imagebinarizationoptions/)
* 部件 [Aspose.Note](../../../)


