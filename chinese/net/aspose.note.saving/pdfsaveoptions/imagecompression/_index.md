---
title: "PdfSaveOptions.ImageCompression"
second_title: "Aspose.Note for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置应用于 PDF 文件中图像的压缩类型"
type: docs
weight: 20
url: /zh/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

获取或设置应用于 PDF 文件中图像的压缩类型。

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


