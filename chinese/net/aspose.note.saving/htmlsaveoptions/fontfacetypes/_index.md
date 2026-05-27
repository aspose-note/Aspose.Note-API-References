---
title: "HtmlSaveOptions.FontFaceTypes"
second_title: "Aspose.Note for .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置字体面类型"
type: docs
weight: 80
url: /zh/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

获取或设置字体类型。

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Property Value

字体面类型。

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

展示如何使用用户定义的回调函数，以 html 格式保存文档并存储所有资源（css/字体/图像）。

```csharp
// 下面的代码创建了 'documentFolder' 文件夹，其中包含 document.html，'css' 文件夹内有 'style.css' 文件，'images' 文件夹内有图像，'fonts' 文件夹内有字体。
// 'style.css' 文件将在末尾包含以下字符串 "/* This line is appended to stream manually by user */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### 另请参阅

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Note.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Note](../../../)


