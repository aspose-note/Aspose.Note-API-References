---
title: Title
second_title: Aspose.Note for .NET API 参考
description: 代表一个标题
type: docs
weight: 950
url: /zh/net/aspose.note/title/
---
## Title class

代表一个标题。

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Title](title#constructor)() | 初始化[`Title`](../title)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset) { get; set; } | 获取或设置水平偏移量。 |
| override [IsComposite](../../aspose.note/title/iscomposite) { get; } | 获取一个值，该值指示此节点是否为复合节点。如果为真，则节点可以有子节点。 |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime) { get; set; } | 获取或设置上次修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [TitleDate](../../aspose.note/title/titledate) { get; set; } | 获取或设置标题中日期的字符串表示形式。 |
| [TitleText](../../aspose.note/title/titletext) { get; set; } | 获取或设置标题的文本。 |
| [TitleTime](../../aspose.note/title/titletime) { get; set; } | 获取或设置标题中时间的字符串表示形式。 |
| [VerticalOffset](../../aspose.note/title/verticaloffset) { get; set; } | 获取或设置垂直偏移量。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/title/accept)(DocumentVisitor) | 接受节点的访问者。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes#getchildnodes_1)() | 按节点类型获取所有子节点。 |
| [GetEnumerator](../../aspose.note/title/getenumerator)() | 返回一个遍历子节点的枚举器[`Title`](../title). |

### 例子

显示如何编辑页面的历史记录。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个孩子           
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

显示如何为页面设置标题。

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

展示如何使用默认选项创建文档并以 html 格式保存。

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

演示如何创建文档并以 html 格式保存指定范围的页面。

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

显示如何创建带有标题页的文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Aspose.Note.Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 设置页面标题属性
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 在文档中追加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

显示如何以不同格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化新文档
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 初始化新页面
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 追加页面节点
doc.AppendChildLast(page);

// 以不同格式保存 OneNote 文档，设置文本字体大小并手动检测布局变化。
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### 也可以看看

* class [CompositeNodeBase](../compositenodebase)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1)
* class [RichText](../richtext)
* interface [IPageChildNode](../ipagechildnode)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
