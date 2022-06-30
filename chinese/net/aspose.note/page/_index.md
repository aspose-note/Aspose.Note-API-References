---
title: Page
second_title: Aspose.Note for .NET API 参考
description: 代表一个页面
type: docs
weight: 460
url: /zh/net/aspose.note/page/
---
## Page class

代表一个页面。

```csharp
public sealed class Page : CompositeNode<IPageChildNode>
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Page](page#constructor)() | 初始化[`Page`](../page)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Author](../../aspose.note/page/author) { get; set; } | 获取或设置作者。 |
| [BackgroundColor](../../aspose.note/page/backgroundcolor) { get; set; } | 获取或设置页面的背景颜色。 |
| [CreationTime](../../aspose.note/page/creationtime) { get; set; } | 获取或设置创建时间。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [IsConflictPage](../../aspose.note/page/isconflictpage) { get; set; } | 获取或设置一个值，该值指示该页面是否为冲突页面。 |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/page/lastmodifiedtime) { get; set; } | 获取或设置最后修改时间。 |
| [Level](../../aspose.note/page/level) { get; set; } | 获取或设置级别。 |
| [Margin](../../aspose.note/page/margin) { get; set; } | 获取或设置边距。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [PageContentRevisionSummary](../../aspose.note/page/pagecontentrevisionsummary) { get; set; } | 获取或设置页面及其子节点的修订摘要。 |
| [PageLayoutSize](../../aspose.note/page/pagelayoutsize) { get; set; } | 获取或设置页面在编辑器中显示的布局大小。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [SizeType](../../aspose.note/page/sizetype) { get; set; } | 获取或设置页面的大小类型。 |
| [Title](../../aspose.note/page/title) { get; set; } | 获取或设置标题。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/page/accept)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [Clone](../../aspose.note/page/clone)(bool) | 克隆页面。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/page/getchildnodes#getchildnodes_1)() | 按节点类型获取页面的所有子节点。 |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IPageChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IPageChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### 例子

显示如何设置页面的背景颜色。

```csharp
//------------------------
string dataDir = RunExamples.GetDataDir_Pages();

//------------------------           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

```csharp
//------------------------
string dataDir = RunExamples.GetDataDir_Pages();

// 保存 OneNote 文档
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
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

```csharp
// 创建 Document 类的对象
string dataDir = RunExamples.GetDataDir_Pages();

//初始化Page类对象
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 初始化大纲类对象
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
// 初始化 TextStyle 类对象并设置格式属性
string dataDir = RunExamples.GetDataDir_Pages();

// 初始化 OutlineElement 类对象并应用项目符号           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// 初始化 RichText 类对象并应用文本样式
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// 添加轮廓元素
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

```csharp
// 添加大纲节点
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// 添加页面节点
Document oneFile = new Document(dataDir + "Aspose.one");

// 保存 OneNote 文档
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 创建 Document 类的对象
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

//初始化Page类对象
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// 初始化大纲类对象
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// 初始化 TextStyle 类对象并设置格式属性
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// 初始化 OutlineElement 类对象并应用编号
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 同一大纲中的数字会自动递增。
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// 添加轮廓元素
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// 添加大纲节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 添加页面节点
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 保存 OneNote 文档
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 文档目录的路径。
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// 加载 OneNote 文档并获取第一个孩子
string dataDir = RunExamples.GetDataDir_Tags();

// 文档目录的路径。
Document doc = new Document();

// 将文档加载到 Aspose.Note。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档目录的路径。
Outline outline = new Outline(doc);

// 加载 OneNote 文档
OutlineElement outlineElem = new OutlineElement(doc);

// 获取第一页
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// 文档目录的路径。
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// 加载 OneNote 文档并获取第一个孩子
outline.AppendChildLast(outlineElem);

// 阅读本页的内容修订摘要
page.AppendChildLast(outline);

// 更新此页面的页面修订摘要
doc.AppendChildLast(page);

// 文档目录的路径。
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// 将文档加载到 Aspose.Note。
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

    // 获取所有富文本节点
    // 替换形状的文本
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

```csharp
// 保存为任何支持的文件格式
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 将文档加载到 Aspose.Note。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 获取所有富文本节点
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 替换形状的文本
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存为任何支持的文件格式
Document doc = new Aspose.Note.Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 OneNote 文档
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档中所有文本的默认样式。
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 保存为 HTML 格式
doc.AppendChildLast(page);

// 文档目录的路径。
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

```csharp
// 创建 Document 类的对象
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

//初始化Page类对象
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 初始化大纲类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 OutlineElement 类对象
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 加载一张图片
doc.AppendChildLast(page);

// 在文档节点中插入图片
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加大纲元素节点
Aspose.Note.Document doc = new Aspose.Note.Document();

// 添加大纲节点
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 添加页面节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档目录的路径。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 加载 OneNote 文档
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 加载 OneNote 文档
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 加载 OneNote 文档
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 文档目录的路径。
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OneNote 文档
Aspose.Note.Document doc = new Aspose.Note.Document();

// 文档中所有文本的默认样式。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 保存为 HTML 格式
Outline outline = new Outline(doc);

// 文档目录的路径。
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 创建 Document 类的对象
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

//初始化Page类对象
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 文档中所有文本的默认样式。
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 设置页面标题属性
page.AppendChildLast(outline);
// 在文档中追加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 文档目录的路径。
Document doc = new Document();

// 初始化新文档
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化新页面
Outline outline = new Outline(doc);

// 文档中所有文本的默认样式。
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 追加页面节点
// 以不同格式保存 OneNote 文档，设置文本字体大小并手动检测布局变化。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 初始化 OneNote 文档
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 初始化 OneNote 页面
page.AppendChildLast(outline);

// 应用文本样式设置
doc.AppendChildLast(page);

// 同一大纲中的数字会自动递增。
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
//------------------------
string dataDir = RunExamples.GetDataDir_Pages();

//------------------------
Document doc = new Document();

//------------------------
Aspose.Note.Page page1 = new Aspose.Note.Page(doc) { Level = 1 };

//------------------------
Aspose.Note.Page page2 = new Aspose.Note.Page(doc) { Level = 2 };

//------------------------
Aspose.Note.Page page3 = new Aspose.Note.Page(doc) { Level = 1 };

/*---------- Adding nodes to first Page ----------*/
Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "First page.", ParagraphStyle = textStyle };
outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page1.AppendChildLast(outline);

/*---------- Adding nodes to second Page ----------*/
var outline2 = new Outline(doc);
var outlineElem2 = new OutlineElement(doc);
var textStyle2 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text2 = new RichText(doc) { Text = "Second page.", ParagraphStyle = textStyle2 };
outlineElem2.AppendChildLast(text2);
outline2.AppendChildLast(outlineElem2);
page2.AppendChildLast(outline2);

/*---------- Adding nodes to third Page ----------*/
var outline3 = new Outline(doc);
var outlineElem3 = new OutlineElement(doc);
var textStyle3 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text3 = new RichText(doc) { Text = "Third page.", ParagraphStyle = textStyle3 };
outlineElem3.AppendChildLast(text3);
outline3.AppendChildLast(outlineElem3);
page3.AppendChildLast(outline3);

/*---------- Add pages to the OneNote Document ----------*/
doc.AppendChildLast(page1);
doc.AppendChildLast(page2);
doc.AppendChildLast(page3);

//初始化Page类对象
dataDir = dataDir + "CreateDocWithRootAndSubPages_out.one";
doc.Save(dataDir);
```

显示如何获取有关页面的元信息。

显示如何为页面设置标题。

显示如何获取页面的历史记录。

显示如何编辑页面的元信息。

显示如何通过所有页面并在文本中进行替换。

显示如何通过页面文本并进行替换。

显示如何使用默认选项创建文档并将其保存为 html 格式。

显示如何添加带有标签的新图像。

显示如何检查页面是否为冲突页面（即它具有 OneNote 无法自动合并的更改）。

显示如何创建文档并以 html 格式保存指定范围的页面。

显示如何创建带有标题页的文档。

显示如何以不同格式保存文档。

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

显示如何添加带有子页面的页面。

### 也可以看看

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IPageChildNode](../ipagechildnode)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
