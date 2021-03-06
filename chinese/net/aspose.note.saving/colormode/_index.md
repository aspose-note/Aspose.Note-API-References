---
title: ColorMode
second_title: Aspose.Note for .NET API 参考
description: 图像的颜色模式
type: docs
weight: 550
url: /zh/net/aspose.note.saving/colormode/
---
## ColorMode enumeration

图像的颜色模式。

```csharp
public enum ColorMode
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| Normal | `0` | 全彩图像 |
| GrayScale | `1` | 灰度图像 |
| BlackAndWhite | `2` | 二进制图像:仅使用黑色和白色 |

### 例子

显示如何将文档保存为灰度图像。

```csharp
// 保存 OneNote 文档
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// 创建 Document 类的对象
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

```csharp
// 添加轮廓元素
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化 Title 类对象
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

//初始化Page类对象
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

```csharp
// 添加大纲节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 添加页面节点
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// 保存 OneNote 文档
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
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// 获取所有富文本节点
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

显示如何使用 CCITT Group 3 传真压缩将文档保存为 Tiff 格式的图像。

显示如何使用 Otsu 的方法将文档保存为二进制图像。

显示如何使用固定阈值将文档保存为二进制图像。

### 也可以看看

* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
