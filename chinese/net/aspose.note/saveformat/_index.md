---
title: SaveFormat
second_title: Aspose.Note for .NET API 参考
description: 表示文档保存的格式
type: docs
weight: 520
url: /zh/net/aspose.note/saveformat/
---
## SaveFormat enumeration

表示文档保存的格式。

```csharp
public enum SaveFormat
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| Png | `1` | 指定输出为 PNG 文件。 |
| Bmp | `2` | 指定输出为 BMP 文件。 |
| Jpeg | `3` | 指定输出为 JPEG 文件。 |
| Gif | `4` | 指定输出为 GIF 文件。 |
| Tiff | `5` | 指定输出为 TIFF 文件。 |
| Pdf | `6` | 指定输出为 PDF 文件。 |
| One | `7` | 指定输出是 OneNote 文件。 |
| Html | `8` | 指定输出是 HTML 文件。 |

### 例子

显示如何使用 SaveFormat 枚举保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

```csharp
// 保存为 HTML 格式
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// 将文档加载到 Aspose.Note。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// 将文档加载到 Aspose.Note。
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

```csharp
// 保存文档。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// 将文档加载到 Aspose.Note。
oneFile.Save(dataDir, SaveFormat.Gif);
```

```csharp
// 将文档加载到 Aspose.Note。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 将文档加载到 Aspose.Note。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// 将文档加载到 Aspose.Note。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 或者
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 或者
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// 加载 OneNote 笔记本
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

```csharp
// 保存笔记本
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// 文档目录的路径。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 或者
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// 或者
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 或者
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// 文档目录的路径。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

```csharp
// 将文档保存为 PDF
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档保存为 PDF
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// 文档目录的路径。
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
// 保存文档。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存文档。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// 文档目录的路径。
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

显示如何使用默认设置以 pdf 格式保存文档。

展示如何使用 SaveFormat 将文档保存为 Jpeg 格式的图像。

显示如何以 gif 格式保存文档。

显示将文档保存为 JPEG 格式的图像时如何设置图像质量。

显示如何使用 ImageSaveOptions 将文档保存为 Bmp 格式的图像。

显示如何在将文档另存为图像时设置图像分辨率。

显示如何将文档保存为灰度图像。

展示如何使用 PackBits 压缩将文档保存为 Tiff 格式的图像。

展示如何使用 Jpeg 压缩将文档保存为 Tiff 格式的图像。

显示如何使用 CCITT Group 3 传真压缩将文档保存为 Tiff 格式的图像。

显示如何使用 Otsu 的方法将文档保存为二进制图像。

显示如何使用固定阈值将文档保存为二进制图像。

### 也可以看看

* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
