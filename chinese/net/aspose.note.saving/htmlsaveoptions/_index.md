---
title: HtmlSaveOptions
second_title: Aspose.Note for .NET API 参考
description: 允许在将文档保存为 HTML 格式时指定其他选项
type: docs
weight: 680
url: /zh/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

允许在将文档保存为 HTML 格式时指定其他选项。

```csharp
public class HtmlSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration) { get; set; } | 获取或设置是否为每个新页面分别生成样式表文件。 |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback) { get; set; } | 获取或设置为创建存储 CSS 的资源而调用的回调。 |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration) { get; set; } | 获取或设置一个值，该值指示是否启用每页生成文档。 |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss) { get; set; } | 获取或设置 css 的导出方式。 |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts) { get; set; } | 获取或设置字体的导出方式。 |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages) { get; set; } | 获取或设置图像的导出方式。 |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes) { get; set; } | 获取或设置字体类型。 |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | 获取或设置为创建资源存储字体而调用的回调。 |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | 获取或设置保存时要使用的字体设置 |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | 获取或设置为创建资源存储图像而调用的回调。 |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | 获取或设置要保存的页数。默认情况下是MaxValue 这意味着将呈现文档的所有页面。 |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | 获取或设置要保存的第一页的索引。默认为 0。 |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | 获取或设置创建资源存储页面调用的回调。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | 获取文档保存的格式。 |

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

```csharp
// 替换形状的文本
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存为任何支持的文件格式
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 将模板文档加载到 Aspose.Note。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 让我们替换所有的模板词
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
替换所有模板词
// 文档目录的路径。
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

展示如何以嵌入所有资源（css/字体/图像）的 html 格式将文档保存到流中。

显示如何创建文档并以 html 格式保存指定范围的页面。

展示如何使用用户定义的回调将文档保存为 html 格式并存储所有资源（css/字体/图像）。

### 也可以看看

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
