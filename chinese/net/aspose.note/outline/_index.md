---
title: Outline
second_title: Aspose.Note for .NET API 参考
description: 表示大纲
type: docs
weight: 430
url: /zh/net/aspose.note/outline/
---
## Outline class

表示大纲。

```csharp
public sealed class Outline : CompositeNode<IOutlineChildNode>, IPageChildNode
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Outline](outline#constructor)() | 初始化[`Outline`](../outline)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved) { get; set; } | 获取大纲的后代是否可以移动。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset) { get; set; } | 获取或设置水平偏移。 |
| [IndentPosition](../../aspose.note/outline/indentposition) { get; set; } | 获取或设置缩进位置。 |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime) { get; set; } | 获取或设置最后修改时间。 |
| [MaxHeight](../../aspose.note/outline/maxheight) { get; set; } | 获取或设置最大高度。 |
| [MaxWidth](../../aspose.note/outline/maxwidth) { get; set; } | 获取或设置最大宽度。 |
| [MinWidth](../../aspose.note/outline/minwidth) { get; set; } | 获取或设置最小宽度。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [ReservedWidth](../../aspose.note/outline/reservedwidth) { get; set; } | 获取或设置保留宽度。 |
| [VerticalOffset](../../aspose.note/outline/verticaloffset) { get; set; } | 获取或设置垂直偏移量。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### 例子

显示如何添加带有标签的新图像。

```csharp
// 保存笔记本
string dataDir = RunExamples.GetDataDir_Tags();

// 默认情况下，子加载是“惰性的”。
Document doc = new Document();

// 因此对于即时加载已经发生，
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 需要设置 NotebookLoadOptions.InstantLoading 标志。
Outline outline = new Outline(doc);

// 所有子文档都已加载。
OutlineElement outlineElem = new OutlineElement(doc);

// 对子文档做一些事情
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// 文档目录的路径。
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// 对子文档做一些事情
outline.AppendChildLast(outlineElem);

// 对子笔记本做一些事情
page.AppendChildLast(outline);

// 文档目录的路径。
doc.AppendChildLast(page);

// 加载 OneNote 笔记本
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 遍历它的子节点，寻找想要的子项
Aspose.Note.Document doc = new Aspose.Note.Document();

// 从笔记本中删除子项
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 保存笔记本
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档目录的路径。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 加载 OneNote 笔记本
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 加载 OneNote 笔记本
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 加载 OneNote 笔记本
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 保存笔记本
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 文档目录的路径。
Aspose.Note.Document doc = new Aspose.Note.Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档目录的路径。
Outline outline = new Outline(doc);

// 文档目录的路径。
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档目录的路径。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 文档目录的路径。
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 创建 Document 类的对象
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

//初始化Page类对象
page.AppendChildLast(outline);
// 初始化大纲类对象
doc.AppendChildLast(page);

// 初始化 OutlineElement 类对象
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 加载一张图片
Document doc = new Document();

// 在文档节点中插入图片
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加大纲元素节点
Outline outline = new Outline(doc);

// 初始化 OneNote 页面
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 应用文本样式设置
// 同一大纲中的数字会自动递增。
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

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

### 也可以看看

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IOutlineChildNode](../ioutlinechildnode)
* interface [IPageChildNode](../ipagechildnode)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
