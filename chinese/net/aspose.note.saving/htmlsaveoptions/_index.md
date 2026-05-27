---
title: "类 HtmlSaveOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.HtmlSaveOptions 类。允许在将文档保存为 HTML 格式时指定其他选项"
type: docs
weight: 780
url: /zh/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

允许在将文档保存为 HTML 格式时指定其他选项。

```csharp
public class HtmlSaveOptions : SaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | 获取或设置是否为每个新页面单独生成 StyleSheet 文件。 |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | 获取或设置用于创建存储 CSS 资源的回调。 |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | 获取或设置一个值，指示是否启用每页生成文档。 |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | 获取或设置 CSS 的导出方式。 |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | 获取或设置字体的导出方式。 |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | 获取或设置图像的导出方式。 |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | 获取或设置字体类型。 |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | 获取或设置用于创建存储字体资源的回调。 |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 获取或设置在保存时使用的字体设置 |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | 获取或设置用于创建存储图像资源的回调。 |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 获取或设置要保存的页数。默认值为 MaxValue，表示将渲染文档的所有页面。 |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 获取或设置要保存的第一页的索引。默认值为 0。 |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | 获取或设置用于创建存储页面资源的回调。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | 获取文档保存的格式。 |

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

展示如何创建文档并在指定页面范围内以 HTML 格式保存。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化 OneNote 文档
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 保存为 HTML 格式
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
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

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


