---
title: "ImageSaveOptions.Quality"
second_title: "Aspose.Note for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置决定已保存图像质量的值。该值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器"
type: docs
weight: 40
url: /zh/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

获取或设置决定已保存图像质量的值。该值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器。

```csharp
public int Quality { get; set; }
```

## 备注

质量类别的有效取值范围为 0 到 100。指定的数值越低，压缩率越高，图像质量因此越低。0 会得到最低质量的图像，100 则为最高质量。默认值为 90。

## 示例

展示如何在将文档保存为 JPEG 图像时设置图像质量。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

展示如何使用 JPEG 压缩将文档保存为 TIFF 格式的图像。

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

### 另请参阅

* class [ImageSaveOptions](../)
* namespace [Aspose.Note.Saving](../../imagesaveoptions/)
* assembly [Aspose.Note](../../../)


