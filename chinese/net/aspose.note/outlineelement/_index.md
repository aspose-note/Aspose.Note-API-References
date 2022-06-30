---
title: OutlineElement
second_title: Aspose.Note for .NET API 参考
description: 表示一个 OutlineElement
type: docs
weight: 440
url: /zh/net/aspose.note/outlineelement/
---
## OutlineElement class

表示一个 OutlineElement。

```csharp
public sealed class OutlineElement : CompositeNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [OutlineElement](outlineelement#constructor)() | 初始化[`OutlineElement`](../outlineelement)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CreationTime](../../aspose.note/outlineelement/creationtime) { get; set; } | 获取或设置创建时间。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IndentPosition](../../aspose.note/outlineelement/indentposition) { get; set; } | 获取或设置缩进位置。 |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime) { get; set; } | 获取或设置最后修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [NumberList](../../aspose.note/outlineelement/numberlist) { get; set; } | 获取或设置编号列表标题的样式。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineElementChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### 例子

显示如何添加带有标签的新图像。

```csharp
//------------------------
string dataDir = RunExamples.GetDataDir_Tags();

//------------------------
Document doc = new Document();

//------------------------
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加轮廓元素
Outline outline = new Outline(doc);

// 创建 Document 类的对象
OutlineElement outlineElem = new OutlineElement(doc);

//初始化Page类对象
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// 初始化大纲类对象
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// 初始化 TextStyle 类对象并设置格式属性
outline.AppendChildLast(outlineElem);

// 初始化 OutlineElement 类对象并应用项目符号
page.AppendChildLast(outline);

// 初始化 RichText 类对象并应用文本样式
doc.AppendChildLast(page);

// 添加轮廓元素
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加大纲节点
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// 添加页面节点
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 保存 OneNote 文档
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 创建 Document 类的对象
        Console.WriteLine("Font Name: " + list.Font);

        //初始化Page类对象
        Console.WriteLine("Font Length: " + list.Font.Length);

        // 初始化大纲类对象
        Console.WriteLine("Font Size: " + list.FontSize);

        // 初始化 TextStyle 类对象并设置格式属性
        Console.WriteLine("Font Color: " + list.FontColor);

        // 初始化 OutlineElement 类对象并应用编号
        Console.WriteLine("Font format: " + list.Format);

        // 同一大纲中的数字会自动递增。
        Console.WriteLine("Is bold: " + list.IsBold);

        // 添加轮廓元素
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加大纲节点
Aspose.Note.Document doc = new Aspose.Note.Document();

// 添加页面节点
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档目录的路径。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 创建 Document 类的对象
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 创建 Document 类的对象
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 创建 Document 类的对象
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 初始化 OutlineElement 类对象
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 加载一张图片
Aspose.Note.Document doc = new Aspose.Note.Document();

// 在文档节点中插入图片
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加大纲元素节点
Outline outline = new Outline(doc);

// 获取大纲元素的集合节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 遍历每个节点
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 获取字体名称
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 将文档加载到 Aspose.Note。
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 获取大纲元素的集合节点
page.AppendChildLast(outline);
// 遍历每个节点
doc.AppendChildLast(page);

// 获取字体名称
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 获取字体长度
Document doc = new Document();

// 获取字体大小
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 获取字体颜色
Outline outline = new Outline(doc);

// 获取格式
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 检查粗体
// 检查斜体
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

显示如何检索有关列表格式的信息。

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

### 也可以看看

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IOutlineChildNode](../ioutlinechildnode)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
