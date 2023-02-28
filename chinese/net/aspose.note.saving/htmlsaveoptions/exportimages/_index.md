---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note for .NET API 参考
description: HtmlSaveOptions 财产. 获取或设置图片的导出方式
type: docs
weight: 70
url: /zh/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

获取或设置图片的导出方式。

```csharp
public ResourceExportType ExportImages { get; set; }
```

### 例子

显示如何将文档保存为 html 格式，并将所有资源（css/字体/图像）存储到单独的文件中。

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

显示如何将文档保存到 html 格式的流中，并嵌入所有资源（css/字体/图像）。

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

### 也可以看看

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 部件 [Aspose.Note](../../../)


