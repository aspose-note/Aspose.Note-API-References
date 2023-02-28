---
title: Enum TiffCompression
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Saving.TiffCompression 枚举. 指定将文档保存为 TIFF 格式时使用的压缩类型
type: docs
weight: 880
url: /zh/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

指定将文档保存为 TIFF 格式时使用的压缩类型。

```csharp
public enum TiffCompression
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| None | `1` | 指定不压缩。 |
| Rle | `2` | 指定 RLE 压缩。 |
| Ccitt3 | `3` | 指定 CCITT Group 3 传真编码。 |
| Ccitt4 | `4` | 指定 CCITT Group 4 传真编码。 |
| Lzw | `5` | 指定 LZW 压缩。 |
| PackBits | `32773` | 指定 Macintosh RLE 压缩。 |
| Jpeg | `7` | 指定JPEG DCT压缩压缩。 |

### 例子

演示如何使用 PackBits 压缩将文档另存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
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

显示如何使用 CCITT Group 3 传真压缩将文档另存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### 也可以看看

* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving/)
* 部件 [Aspose.Note](../../)


