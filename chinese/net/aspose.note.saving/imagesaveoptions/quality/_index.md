---
title: ImageSaveOptions.Quality
second_title: Aspose.Note for .NET API 参考
description: ImageSaveOptions 财产. 获取或设置确定已保存图像质量的值 此值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器
type: docs
weight: 40
url: /zh/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

获取或设置确定已保存图像质量的值。 此值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器。

```csharp
public int Quality { get; set; }
```

### 评论

质量类别的有用值范围是从 0 到 100。 指定的数字越小，压缩率越高，因此图像质量越低。 零将为您提供最低质量的图像，100 为您提供最高质量的图像. 默认值为 90.

### 例子

显示将文档另存为 JPEG 格式图像时如何设置图像质量。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

展示如何使用 Jpeg 压缩将文档另存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### 也可以看看

* class [ImageSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../imagesaveoptions/)
* 部件 [Aspose.Note](../../../)


