---
title: ImageSaveOptions
second_title: Aspose.Note for .NET API 参考
description: 允许在将文档页面呈现为图像时指定其他选项
type: docs
weight: 700
url: /zh/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

允许在将文档页面呈现为图像时指定其他选项。

```csharp
public class ImageSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions)(SaveFormat) | 初始化[`ImageSaveOptions`](../imagesaveoptions)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions) { get; set; } | 获取或设置图像二值化选项。 |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode) { get; set; } | 获取或设置[`ColorMode`](./colormode)对于输出图像. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | 获取或设置保存时要使用的字体设置 |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | 获取或设置要保存的页数。默认情况下是MaxValue 表示将呈现文档的所有页面。 |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | 获取或设置要保存的第一页的索引。默认为 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality) { get; set; } | 获取或设置一个确定保存图像质量的值。 该值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器。 |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution) { get; set; } | 获取或设置生成图像的分辨率，以每英寸点数为单位。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | 获取文档保存的格式。 |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression) { get; set; } | 获取或设置将生成的图像保存为 TIFF 格式时使用的压缩类型。 |

### 例子

演示如何使用 SaveFormat 将文档保存为 Jpeg 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// 保存文档。
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

显示将文档另存为 JPEG 格式的图像时如何设置图像质量。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

演示如何使用 ImageSaveOptions 将文档保存为 Bmp 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// 保存文档。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

显示将文档另存为图像时如何设置图像分辨率。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

显示如何将文档另存为灰度图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// 将文档保存为 gif。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

演示如何使用 PackBits 压缩将文档另存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

显示如何使用指定选项将笔记本保存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

演示如何使用 Jpeg 压缩将文档保存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

显示如何将展平的笔记本另存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

展示如何使用 CCITT Group 3 传真压缩将文档保存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

显示如何以 png 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

// 初始化 ImageSaveOptions 对象 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // 设置页面索引
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// 将文档保存为 PNG。
oneFile.Save(dataDir, opts);
```

展示如何使用 Otsu 的方法将文档保存为二进制图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
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

展示如何使用固定阈值将文档保存为二进制图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
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

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
