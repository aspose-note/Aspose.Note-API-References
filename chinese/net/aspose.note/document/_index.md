---
title: Document
second_title: Aspose.Note for .NET API 参考
description: 表示一个 Aspose.Note 文档
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

| 姓名 | 描述 |
| --- | --- |
| [Document](document#constructor)() | 初始化[`Document`](../document)类的新实例。 创建一个空白的 OneNote 文档。 |
| [Document](document#constructor_1)(Stream) | 初始化[`Document`](../document)类的新实例。 从流中打开现有 OneNote 文档。 |
| [Document](document#constructor_3)(string) | 初始化[`Document`](../document)类的新实例。 从文件中打开现有的 OneNote 文档。 |
| [Document](document#constructor_2)(Stream, LoadOptions) | 初始化[`Document`](../document)类的新实例。 从流中打开现有 OneNote 文档。允许指定其他选项，例如加密密码。 |
| [Document](document#constructor_4)(string, LoadOptions) | 初始化[`Document`](../document)类的新实例。 从文件中打开现有的 OneNote 文档。允许指定其他选项，例如加密密码。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | 获取或设置一个值，该值指示 Aspose.Note 是否自动执行布局更改检测。 默认值为` true` 。 |
| [Color](../../aspose.note/document/color) { get; set; } | 获取或设置颜色。 |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | 获取或设置创建时间。 |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | 获取或设置显示名称。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | 获取文件格式（OneNote 2010、OneNote Online）。 |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | 获取对象的全局唯一 ID。 |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | 检测自上次[`DetectLayoutChanges`](./detectlayoutchanges)调用以来对文档布局所做的所有更改。 如果[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled)设置为 true，则在文档导出开始时自动使用。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | 获取[`PageHistory`](../pagehistory)包含文档中呈现的每个页面的完整历史记录（最早在索引 0 处） . 当前页面修订可以通过[`Current`](../pagehistory/current)访问，并且与历史版本的集合分开包含。 |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | 从提供的 PDF 文档中导入一组页面。 |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | 从提供的 PDF 文档中导入一组页面。 |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | 将一组页面合并到文档中。 |
| [Print](../../aspose.note/document/print#print)() | 使用默认打印机打印文档。 |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | 使用默认打印机打印文档。 |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | 将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/document/save#save_3)(string) | 将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | 将 OneNote 文档以指定格式保存到流中。 |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | 使用指定的保存选项将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | 将 OneNote 文档保存到指定格式的文件中。 |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | 使用指定的保存选项将 OneNote 文档保存到文件中。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | 检查流中的文档是否已加密。 要检查它，我们需要完全加载此文档。所以这种方法会导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | 检查文件中的文档是否已加密。 要检查它，我们需要完全加载此文档。所以这种方法会导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | 检查流中的文档是否已加密。 要检查它，我们需要完全加载此文档。所以这种方法会导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | 检查流中的文档是否已加密。 要检查它，我们需要完全加载此文档。所以这种方法会导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | 检查文件中的文档是否已加密。 要检查它，我们需要完全加载此文档。所以这种方法会导致性能损失。 |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | 检查文件中的文档是否已加密。 要检查它，我们需要完全加载此文档。所以这种方法会导致性能损失。 |

### 例子

显示如何使用带有默认选项的标准 Windows 对话框将文档发送到打印机。

```csharp
// 添加页面节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

```csharp
// 保存 OneNote 文档
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

```csharp
// 创建 Document 类的对象
string dataDir = RunExamples.GetDataDir_Pages();

// 添加轮廓元素
Document oneFile = new Document(dataDir + "Aspose.one");

// 初始化 Title 类对象
int count = oneFile.Count();

//初始化Page类对象
Console.WriteLine(count);
```

```csharp
// 添加大纲节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 添加页面节点
Document oneFile = new Document(dataDir + "Aspose.one");

// 保存 OneNote 文档
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// 文档目录的路径。
oneFile.Save(dataDir, SaveFormat.Gif);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 获取页数
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

```csharp
// 在输出屏幕上打印计数
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 将文档加载到 Aspose.Note。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

```csharp
// 将文档保存为 PDF
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // 文档目录的路径。
        break;
    case FileFormat.OneNoteOnline:
        // 将文档加载到 Aspose.Note。
        break;
}
```

```csharp
// 将文档保存为 gif。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http:// 文档目录的路径。

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

```csharp
// 保存文档。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存文档。
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// 文档目录的路径。
dstStream.Seek(0, SeekOrigin.Begin);
```

```csharp
// 将文档加载到 Aspose.Note。
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

```csharp
// 保存文档。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 文档目录的路径。
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 处理 OneNote 2010
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// 在线处理 OneNote
notebook.Save(dataDir);
```

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

```csharp
//image.com" };
string dataDir = RunExamples.GetDataDir_Pages();

// 文档目录的路径。           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

```csharp
// 将文档加载到 Aspose.Note。
string dataDir = RunExamples.GetDataDir_Pages();

// 将流位置倒回零，以便为下一个阅读器做好准备。
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 文档目录的路径。
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// 文档目录的路径。
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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
// 加载 OneNote 笔记本
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

```csharp
// 添加一个新的子节点到 Notebook
string dataDir = RunExamples.GetDataDir_Pages();

// 保存笔记本
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

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// 加载 OneNote 文档并获取第一个孩子
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 加载 OneNote 文档
Document oneFile = new Document(dataDir + "Aspose.one");

// 克隆到没有历史记录的新文档 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // 克隆到具有历史记录的新文档
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// 文档目录的路径。
oneFile.Save(dataDir, opts);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 将文档加载到 Aspose.Note。           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

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

```csharp
// 将文档加载到 Aspose.Note。
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
            // 或者
        }
        else if (notebookChildNode is Notebook)
        {
            // 文档目录的路径。
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

```csharp
// 初始化 ImageSaveOptions 对象
string dataDir = RunExamples.GetDataDir_Images();

// 初始化 ImageSaveOptions 对象
Document oneFile = new Document(dataDir + "Aspose.one");

// 设置页面索引
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 将文档保存为 PNG。
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 加载 OneNote 文档并获取第一个孩子
Document oneFile = new Document(dataDir + "Aspose.one");

// 文档目录的路径。
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 文档目录的路径。
                              PageIndex = 0,

                              // 对子文档做一些事情
                              PageCount = 1,
                          };

// 对子笔记本做一些事情
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document(dataDir + "Aspose.one");

// 获取所有图像节点
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 将图像字节保存到文件中
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // 文档目录的路径。
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

```csharp
// 将文档加载到 Aspose.Note。
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

```csharp
// 初始化 PdfSaveOptions 对象
string dataDir = RunExamples.GetDataDir_Images();

// 设置要保存的第一页的页索引
Document oneFile = new Document(dataDir + "Aspose.one");

// 设置页数
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

```csharp
// 将文档保存为 PDF
string dataDir = RunExamples.GetDataDir_Attachments();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Sample1.one");

// 将文档加载到 Aspose.Note。
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// 初始化 PdfSaveOptions 对象
foreach (AttachedFile file in nodes)
{
    // 使用 Jpeg 压缩
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // JPEG 压缩的质量
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // 文档目录的路径。
            CopyStream(outputStream, fileStream);
        }
    }
}
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 获取所有图像节点
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

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 将文档加载到 Aspose.Note。
Document doc = new Document();

// 获取附件节点列表
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 遍历所有节点
Outline outline = new Outline(doc);

// 将附件加载到流对象
OutlineElement outlineElem = new OutlineElement(doc);

// 创建本地文件
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// 复制文件流
outlineElem.AppendChildLast(attachedFile);

// 文档目录的路径。
outline.AppendChildLast(outlineElem);

// 加载 OneNote 文档
page.AppendChildLast(outline);

// 获取第一页
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

//初始化Page类对象
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 初始化大纲类对象
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// 初始化 OutlineElement 类对象
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

    // 初始化 AttachedFile 类对象
    // 添加附件
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

```csharp
// 添加大纲元素节点
string dataDir = RunExamples.GetDataDir_Images();

// 添加大纲节点
Document doc = new Document(dataDir + "Aspose.one");

// 添加页面节点
Aspose.Note.Page page = doc.FirstChild;

// 文档目录的路径。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 初始化 OneNote 文档
                              Width = 100,
                              Height = 100,

                              // 文档中所有文本的默认样式。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 保存为 HTML 格式
                              Alignment = HorizontalAlignment.Right
                          };

// 加载 OneNote 文档
page.AppendChildLast(image);
```

```csharp
// 默认情况下，冲突页面只是在保存时跳过。
string dataDir = RunExamples.GetDataDir_Attachments();

// 如果将其标记为非冲突，那么它将像往常一样保存在历史记录中。
Document doc = new Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 从流中加载文档。
Outline outline = new Outline(doc);

// 获取文档的第一页。
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // 从文件中加载图像。
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 根据您的需要更改图像的大小（可选）。
    outlineElem.AppendChildLast(attachedFile);
}

// 设置图片在页面中的位置（可选）。
outline.AppendChildLast(outlineElem);

// 设置图像对齐
page.AppendChildLast(outline);

// 将图像添加到页面。
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

```csharp
s 尺寸根据您的需要（可选）。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

页面中的位置（可选）。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 文档目录的路径。
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 文档目录的路径。
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 文档目录的路径。
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 文档目录的路径。
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

```csharp
// 初始化 OutlineElement 类对象
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化 AttachedFile 类对象并传递其图标路径
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 添加附件
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 添加大纲元素节点
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 添加大纲节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 添加页面节点
Document doc = new Aspose.Note.Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 将文档加载到 Aspose.Note。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 或者
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 或者
doc.AppendChildLast(page);

// 或者
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_Images();

// 文档目录的路径。
Document doc = new Document();

// 初始化 OneNote 文档
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // 文档中所有文本的默认样式。
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 保存为 HTML 格式
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// 文档目录的路径。
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

```csharp
// 文档中所有文本的默认样式。
string dataDir = RunExamples.GetDataDir_Images();

// 文档中所有文本的默认样式。
Document doc = new Document();

// 文档中所有文本的默认样式。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 设置页面标题属性
Outline outline = new Outline(doc);

// 在文档中追加 Page 节点
OutlineElement outlineElem = new OutlineElement(doc);

// 保存 OneNote 文档
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 文档目录的路径。
                              Alignment = HorizontalAlignment.Right
                          };

// 创建 Document 类的对象
outlineElem.AppendChildLast(image);

//初始化Page类对象
outline.AppendChildLast(outlineElem);

// 使用图像名称、扩展名和流加载第二张图像。
page.AppendChildLast(outline);

// 设置图像对齐
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Page page = new Page(doc);

// 初始化 Outline 类对象并设置偏移属性
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);

// 通过文件路径加载图片。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 设置图像对齐
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// 添加图片
outlineElem.AppendChildLast(text);

// 添加轮廓元素
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 初始化 OutlineElement 类对象
doc.AppendChildLast(page);

// 初始化 TextStyle 类对象并设置格式属性
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

```csharp
// 初始化 RichText 类对象并应用文本样式
// 添加富文本节点
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

```csharp
// 添加 OutlineElement 节点
string dataDir = RunExamples.GetDataDir_Tasks();

// 初始化新文档
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
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 初始化新页面
outline.AppendChildLast(outlineElem);

// 文档中所有文本的默认样式。
Title title = new Title() { TitleText = titleText };

// 文档目录的路径。
Page page = new Note.Page() { Title = title };

// 初始化新文档
page.AppendChildLast(outline);

// 初始化新页面
doc.AppendChildLast(page);

// 文档中所有文本的默认样式。
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

```csharp
public static void Run()
{
    // 添加轮廓元素 追加页面节点
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // 添加轮廓元素 以不同格式保存 OneNote 文档，设置文本字体大小并手动检测布局变化。
    Document doc = new Document(dataDir + "Aspose.one");

    // 添加轮廓元素 下面的代码创建包含 document.html 的“documentFolder”文件夹，包含“style.css”文件的“css”文件夹，包含图像的“images”文件夹和包含字体的“fonts”文件夹。
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // 添加轮廓元素 'style.css' 文件将在末尾包含以下字符串 "/* 此行由用户手动附加到流 */"
    // 添加轮廓元素 文档目录的路径。
    // 添加轮廓元素 创建 Document 类的对象
    // 添加轮廓元素
    // 添加轮廓元素 注意对象模型中的每个节点都有 Accept 方法，所以访问
    // 添加轮廓元素 不仅可以对整个文档执行，还可以对文档中的任何节点执行。
    doc.Accept(myConverter);

    // 添加轮廓元素 一旦访问完成，我们可以检索操作的结果，
    // 添加轮廓元素 在此示例中，已在访问者中累积。
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

// 添加轮廓元素/ <summary>
// 添加轮廓元素/ 以纯文本格式保存文档的简单实现。作为访客实现。
// 添加轮廓元素/ </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 获取访问者积累的文档的纯文本。
    // 添加轮廓元素/ </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 将文本添加到当前输出。尊重启用/禁用的输出标志。
    // 添加轮廓元素/ </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 RichText 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 Document 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 Page 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ Page 节点处理完成时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 Title 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 Image 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 OutlineGroup 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到大纲节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 在文档中遇到 OutlineElement 节点时调用。
    // 添加轮廓元素/ </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    // 添加轮廓元素/ <summary>
    // 添加轮廓元素/ 获取Visitor的节点总数
    // 添加轮廓元素/ </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

显示如何保存文档。

显示如何加密文档。

显示如何使用加密保存文档。

显示如何使用 SaveFormat 枚举保存文档。

显示如何使用 OneSaveOptions 保存文档。

显示如何获取文档的页面计数。

显示如何使用默认设置以 pdf 格式保存文档。

显示如何以 gif 格式保存文档。

显示将文档保存为 JPEG 格式的图像时如何设置图像质量。

显示如何在将文档另存为图像时设置图像分辨率。

显示如何获取文档的文件格式。

显示如何将超链接绑定到图像。

显示如何将文档保存到流中。

显示如何检查文档是否受密码保护。

显示如何将新分区添加到笔记本。

显示如何检查文档加载是否因为不支持 OneNote 2007 格式而失败。

显示如何恢复页面的先前版本。

显示如何克隆页面。

展示如何以 html 格式保存文档，并将所有资源（css/字体/图像）存储到单独的文件中。

展示如何以嵌入所有资源（css/字体/图像）的 html 格式将文档保存到流中。

显示如何设置图像的文本描述。

显示如何获取有关页面的元信息。

当长 OneNote 页面以 pdf 格式保存时，它们会在页面之间拆分。该示例展示了如何配置位于分页符上的对象的拆分逻辑。

显示如何以 png 格式保存文档。

显示如何编辑页面的历史记录。

显示如何检查文档是否受特定密码的密码保护。

显示如何传递笔记本的内容。

显示如何从文档中获取图像。

显示如何以 pdf 格式保存文档。

显示如何使用特定设置以 pdf 格式保存文档。

显示如何使用带有指定选项的标准 Windows 对话框将文档发送到打印机。

显示如何获取图像的元信息。

显示如何获取附件的内容。

显示如何获取页面的历史记录。

显示如何使用文件路径将文件添加到文档中。

显示如何使用默认选项创建文档并将其保存为 html 格式。

显示如何检查页面是否为冲突页面（即它具有 OneNote 无法自动合并的更改）。

显示如何将图像从文件添加到具有用户定义属性的文档。

显示如何将文件从流添加到文档。

当长 OneNote 页面以 pdf 格式保存时，它们会在页面之间拆分。该示例显示了如何配置位于分页符上的对象的拆分逻辑。

显示如何创建文档并以 html 格式保存指定范围的页面。

显示如何创建带有标题页的文档。

显示如何将图像从流添加到文档。

显示如何将图像从文件添加到文档。

显示如何创建带有文本的文档。

显示如何以不同格式保存文档。

展示如何使用用户定义的回调将文档保存为 html 格式并存储所有资源（css/字体/图像）。

显示如何将超链接绑定到文本。

显示如何使用访问者访问文档的内容。

### 也可以看看

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
