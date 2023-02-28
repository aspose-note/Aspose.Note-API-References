---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note for .NET API 参考
description: PdfSaveOptions 财产. 获取或设置确定 PDF 文档中 JPEG 图像质量的值 该值可能在 0 到 100 之间变化其中 0 表示质量最差但压缩最大100 表示质量最好但压缩最小
type: docs
weight: 30
url: /zh/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

获取或设置确定 PDF 文档中 JPEG 图像质量的值。 该值可能在 0 到 100 之间变化，其中 0 表示质量最差但压缩最大，100 表示质量最好但压缩最小。

```csharp
public int JpegQuality { get; set; }
```

### 评论

默认值为 90.

### 例子

显示如何使用特定设置将文档保存为 pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

// 初始化 PdfSaveOptions 对象
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 使用 Jpeg 压缩
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 压缩质量
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### 也可以看看

* class [PdfSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 部件 [Aspose.Note](../../../)


