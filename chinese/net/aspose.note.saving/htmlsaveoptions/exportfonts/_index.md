---
title: "HtmlSaveOptions.ExportFonts"
second_title: "Aspose.Note for .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置字体的导出方式"
type: docs
weight: 60
url: /zh/net/aspose.note.saving/htmlsaveoptions/exportfonts/
---
## HtmlSaveOptions.ExportFonts property

获取或设置字体的导出方式。

```csharp
public ResourceExportType ExportFonts { get; set; }
```

## 示例

展示如何以 HTML 格式保存文档，并将所有资源（css/字体/图像）存储到单独的文件中。

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

展示如何以 HTML 格式将文档保存到流中，并嵌入所有资源（css/字体/图像）。

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

### 另请参阅

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Note.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Note](../../../)


