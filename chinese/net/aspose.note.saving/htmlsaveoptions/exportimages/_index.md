---
title: ExportImages
second_title: Aspose.Note for .NET API 参考
description: 获取或设置图像的导出方式
type: docs
weight: 70
url: /zh/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

获取或设置图像的导出方式。

```csharp
public ResourceExportType ExportImages { get; set; }
```

### 例子

显示如何以 html 格式保存文档，并将所有资源（css/字体/图像）存储到单独的文件中。

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

展示如何以嵌入所有资源（css/字体/图像）的 html 格式将文档保存到流中。

### 也可以看看

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype)
* class [HtmlSaveOptions](../../htmlsaveoptions)
* 命名空间 [Aspose.Note.Saving](../../htmlsaveoptions)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
