---
title: "类 Document"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Document 类。表示 Aspose.Note 文档"
type: docs
weight: 60
url: /zh/net/aspose.note/document/
---
## Document class

表示一个 Aspose.Note 文档。

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Document](document/#constructor)() | 初始化 `Document` 类的新实例。创建一个空白的 OneNote 文档。 |
| [Document](document/#constructor_1)(Stream) | 初始化 `Document` 类的新实例。从流中打开现有的 OneNote 文档。 |
| [Document](document/#constructor_3)(string) | 初始化 `Document` 类的新实例。从文件中打开现有的 OneNote 文档。 |
| [Document](document/#constructor_2)(Stream, LoadOptions) | 初始化 `Document` 类的新实例。从流中打开现有的 OneNote 文档。允许指定额外选项，例如加密密码。 |
| [Document](document/#constructor_4)(string, LoadOptions) | 初始化 `Document` 类的新实例。从文件中打开现有的 OneNote 文档。允许指定额外选项，例如加密密码。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | 获取或设置一个值，指示 Aspose.Note 是否自动检测布局更改。默认值为 `true`。 |
| [Color](../../aspose.note/document/color/) { get; set; } | 获取或设置颜色。 |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | 获取或设置创建时间。 |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | 获取或设置显示名称。 |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | 获取文件格式（OneNote 2010，OneNote Online）。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | 获取对象的全局唯一标识符。 |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | 检测自上一次 [`DetectLayoutChanges`](./detectlayoutchanges/) 调用以来对文档布局所做的所有更改。如果 [`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) 设置为 true，则在文档导出开始时自动使用。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | 获取 [`PageHistory`](../pagehistory/)，它包含文档中每页的完整历史（最早的在索引 0）。当前页面修订版可以通过 [`Current`](../pagehistory/current/) 访问，并且与历史版本集合分开存放。 |
| [Import](../../aspose.note/document/import/#import)(Stream, HtmlImportOptions, MergeOptions) | 从提供的 HTML 文档导入一组页面。 |
| [Import](../../aspose.note/document/import/#import_1)(Stream, PdfImportOptions, MergeOptions) | 从提供的 PDF 文档导入一组页面。 |
| [Import](../../aspose.note/document/import/#import_2)(string, HtmlImportOptions, MergeOptions) | 从提供的 HTML 文档导入一组页面。 |
| [Import](../../aspose.note/document/import/#import_3)(string, PdfImportOptions, MergeOptions) | 从提供的 PDF 文档导入一组页面。 |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | 将一组页面合并到文档中。 |
| [Print](../../aspose.note/document/print/#print)() | 使用默认打印机打印文档。 |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | 使用默认打印机打印文档。 |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | 将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/document/save/#save_3)(string) | 将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | 以指定格式将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | 使用指定的保存选项将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | 以指定格式将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | 使用指定的保存选项将 OneNote 文档保存到文件中。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | 检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | 检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | 检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | 检查来自流的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | 检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | 检查来自文件的文档是否已加密。要进行检查，需要完整加载该文档。因此此方法可能导致性能损失。 |

## 示例

展示如何使用带默认选项的标准 Windows 对话框将文档发送到打印机。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

展示如何保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

展示如何处理加密文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

展示如何使用加密保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

展示如何使用 SaveFormat 枚举保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

展示如何使用 OneSaveOptions 保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

展示如何获取文档的页数。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取页数
int count = oneFile.Count();

// 在输出屏幕上打印计数
Console.WriteLine(count);
```

展示如何使用默认设置将文档保存为 pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 将文档保存为 PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

展示如何将文档保存为 gif 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// 将文档保存为 gif。
oneFile.Save(dataDir, SaveFormat.Gif);
```

展示如何在将文档保存为 JPEG 图像时设置图像质量。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

展示如何在将文档保存为图像时设置图像分辨率。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

展示如何将超链接绑定到图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page();

var image = new Image(dataDir + "image.jpg") { HyperlinkUrl = "https://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

展示如何获取文档的文件格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // 处理 OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // 处理 OneNote Online
        break;
}
```

展示如何将文档保存到流中。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// 将流位置倒回到零，以便下一个读取器使用。
dstStream.Seek(0, SeekOrigin.Begin);
```

展示如何检查文档是否受密码保护。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

展示如何向笔记本添加新章节。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// 向笔记本追加新子项
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// 保存笔记本
notebook.Save(dataDir);
```

展示如何检查文档加载是否因不支持 OneNote 2007 格式而失败。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

展示如何恢复页面的先前版本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子项
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

展示如何克隆页面。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 克隆到新文档（不含历史）
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// 克隆到新文档（含历史）
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

展示如何为图像设置文本描述。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page();
var image = new Image(dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

展示如何获取页面的元信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

当长的 OneNote 页面以 PDF 格式保存时，它们会被拆分到多个页面。示例展示如何配置位于页面换页处对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

展示如何以 PNG 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 初始化 ImageSaveOptions 对象 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // 设置页面索引
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// 将文档保存为 PNG。
oneFile.Save(dataDir, opts);
```

展示如何编辑页面的历史记录。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子项
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page();
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page());

    pageHistory.Insert(1, new Page());

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

展示如何检查文档是否被特定密码保护。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

展示如何对文档应用暗色主题样式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

展示如何遍历笔记本的内容。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // 对子文档进行操作
        }
        else if (notebookChildNode is Notebook)
        {
            // 对子笔记本进行操作
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

展示如何从文档中获取图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有 Image 节点
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 将图像字节保存到文件
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

展示如何以 PDF 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 初始化 PdfSaveOptions 对象
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 设置要保存的第一页的页面索引
                              PageIndex = 0,

                              // 设置页面数量
                              PageCount = 1,
                          };

// 将文档保存为 PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

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

展示如何使用标准 Windows 对话框并指定选项将文档发送到打印机。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

展示如何获取附件文件的内容。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Sample1.one");

// 获取附件文件节点的列表
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// 遍历所有节点
foreach (AttachedFile file in nodes)
{
    // 将附件文件加载到流对象中
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // 创建本地文件
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // 复制文件流
            CopyStream(outputStream, fileStream);
        }
    }
}
```

展示如何获取图像的元信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有 Image 节点
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

展示如何获取页面的历史记录。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 获取第一页
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

展示如何通过文件路径将文件添加到文档中。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();

// 初始化 AttachedFile 类对象
AttachedFile attachedFile = new AttachedFile(dataDir + "attachment.txt");

// 添加附件文件
outlineElem.AppendChildLast(attachedFile);

// 添加大纲元素节点
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

展示如何创建文档并使用默认选项将其保存为 HTML 格式。

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

展示如何检查页面是否为冲突页面（即它包含 OneNote 无法自动合并的更改）。

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // 默认情况下，冲突页面在保存时会被跳过。
    // 如果将其标记为非冲突，则它将在历史记录中像普通页面一样保存。
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

展示如何从文件向文档添加图像，并使用用户定义的属性。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 从流中加载文档。
Document doc = new Document(dataDir + "Aspose.one");

// 获取文档的第一页。
Page page = doc.FirstChild;

// 从文件加载图像。
Image image = new Image(dataDir + "image.jpg")
                          {
                              // 根据需要更改图像的大小（可选）。
                              Width = 100,
                              Height = 100,

                              // 设置图像在页面中的位置（可选）。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 设置图像对齐方式
                              Alignment = HorizontalAlignment.Right
                          };

// 将图像添加到页面。
page.AppendChildLast(image);
```

展示如何从流中将文件添加到文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // 初始化 AttachedFile 类对象并传递其图标路径
    AttachedFile attachedFile = new AttachedFile(dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 添加附件文件
    outlineElem.AppendChildLast(attachedFile);
}

// 添加大纲元素节点
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

展示如何从流向文档添加图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

Outline outline1 = new Outline();
OutlineElement outlineElem1 = new OutlineElement();

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // 使用图像名称、扩展名和流加载第二张图像。
    Image image1 = new Image("Penguins.jpg", fs)
                                   {
                                       // 设置图像对齐方式
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

展示如何创建带标题页面的文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 设置页面标题属性
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 在文档中追加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

当长的 OneNote 页面以 PDF 格式保存时，它们会被拆分到多个页面。示例展示如何配置位于页面换行处对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

展示如何从文件向文档添加图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象并设置偏移属性
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();

// 通过文件路径加载图像。
Image image = new Image(dataDir + "image.jpg")
                          {
                              // 设置图像对齐方式
                              Alignment = HorizontalAlignment.Right
                          };

// 添加图像
outlineElem.AppendChildLast(image);

// 添加大纲元素
outline.AppendChildLast(outlineElem);

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
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

展示如何使用文本创建文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 RichText 类对象并应用文本样式
RichText text = new RichText() { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// 添加 RichText 节点
outlineElem.AppendChildLast(text);

// 添加 OutlineElement 节点
outline.AppendChildLast(outlineElem);

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

展示如何将文档保存为不同的格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化新的 Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 初始化新页面
Page page = new Page();

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 追加页面节点
doc.AppendChildLast(page);

// 以不同格式保存 OneNote 文档，设置文本字体大小并手动检测布局更改。
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

展示如何将超链接绑定到文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 创建 Document 类的对象
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       HyperlinkAddress = "https://www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 添加大纲元素
outline.AppendChildLast(outlineElem);

// 初始化 Title 类对象
Title title = new Title() { TitleText = titleText };

// 初始化 Page 类对象
Page page = new Note.Page() { Title = title };

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

展示如何使用访问者访问文档的内容。

```csharp
public static void Run()
{
    // 文档目录的路径。
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // 打开我们想要转换的文档。
    Document doc = new Document(dataDir + "Aspose.one");

    // 创建一个继承自 DocumentVisitor 类的对象。
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // 这是众所周知的 Visitor 模式。让模型接受访问者。
    // 模型将通过调用相应的方法自行遍历
    // 在访问者对象上（这称为访问）。
    //
    // 请注意，对象模型中的每个节点都有 Accept 方法，因此访问
    // 不仅可以对整个文档执行，也可以对文档中的任何节点执行。
    doc.Accept(myConverter);

    // 一旦访问完成，我们可以检索操作的结果，
    // 在本例中，该结果已在访问者中累积。
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// 简单实现将文档保存为纯文本格式。实现为 Visitor。
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// 获取由访问者累积的文档纯文本。
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// 向当前输出添加文本。遵守已启用/已禁用的输出标志。
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// 当文档中遇到 RichText 节点时调用。
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// 当文档中遇到 Document 节点时调用。
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 Page 节点时调用。
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// 当 Page 节点的处理完成时调用。
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// 当文档中遇到 Title 节点时调用。
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 Image 节点时调用。
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 OutlineGroup 节点时调用。
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 Outline 节点时调用。
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// 当文档中遇到 OutlineElement 节点时调用。
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// 获取 Visitor 的节点总数
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### 另请参阅

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


