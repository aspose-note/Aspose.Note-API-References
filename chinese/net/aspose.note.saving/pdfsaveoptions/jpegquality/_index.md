---
title: "PdfSaveOptions.JpegQuality"
second_title: "Aspose.Note for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置决定 PDF 文档中 JPEG 图像质量的值。该值范围为 0 到 100，其中 0 表示质量最差但压缩率最高，100 表示质量最佳但压缩率最低。"
type: docs
weight: 30
url: /zh/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

获取或设置决定 PDF 文档中 JPEG 图像质量的值。该值范围为 0 到 100，其中 0 表示质量最差但压缩最大，100 表示质量最佳但压缩最小。

```csharp
public int JpegQuality { get; set; }
```

## 备注

默认值为 90。

## 示例

展示如何使用特定设置以 PDF 格式保存文档。

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

### 另请参阅

* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


