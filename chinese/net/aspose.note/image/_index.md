---
title: Image
second_title: Aspose.Note for .NET API 参考
description: 表示一个图像
type: docs
weight: 240
url: /zh/net/aspose.note/image/
---
## Image class

表示一个图像。

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Image](image#constructor)() | 初始化[`Image`](../image)类. |
| [Image](image#constructor_4)(string, Stream) | 初始化[`Image`](../image)类. |
| [Image](image#constructor_5)(string, string, string) | 初始化[`Image`](../image)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment) { get; set; } | 获取或设置对齐方式。 |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription) { get; set; } | 获取或设置正文为图像的替代文本。 |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle) { get; set; } | 获取或设置图像的替代文本标题。 |
| [Bytes](../../aspose.note/image/bytes) { get; } | 获取图像数据存储。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FileName](../../aspose.note/image/filename) { get; } | 获取文件名。 |
| [FilePath](../../aspose.note/image/filepath) { get; } | 获取图像文件的路径。 |
| [Format](../../aspose.note/image/format) { get; } | 获取图像的格式。 |
| [Height](../../aspose.note/image/height) { get; set; } | 获取或设置高度。这是MS OneNote文档中图片的真实高度。 |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset) { get; set; } | 获取或设置水平偏移量。 |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl) { get; set; } | 获取或设置与图像关联的超链接。 |
| [IsBackground](../../aspose.note/image/isbackground) { get; set; } | 获取图片是否为背景图片。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | 获取一个值，该值指示此节点是否为复合节点。如果为真，则节点可以有子节点。 |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime) { get; set; } | 获取或设置上次修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [OriginalHeight](../../aspose.note/image/originalheight) { get; } | 获取原始高度。这是调整大小之前图像的原始宽度。 |
| [OriginalWidth](../../aspose.note/image/originalwidth) { get; } | 获取原始宽度。这是调整大小之前图像的原始宽度。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [Tags](../../aspose.note/image/tags) { get; } | 获取段落的所有标签列表。 |
| [VerticalOffset](../../aspose.note/image/verticaloffset) { get; set; } | 获取或设置垂直偏移量。 |
| [Width](../../aspose.note/image/width) { get; set; } | 获取或设置宽度。这是MS OneNote文档中图片的真实宽度。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/image/accept)(DocumentVisitor) | 接受节点的访问者。 |

### 例子

显示如何将超链接绑定到图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

显示如何为图像设置文本描述。

```csharp
// 文档目录的路径。
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

显示如何从文档中获取图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有图像节点
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 将图像字节保存到文件中
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

显示如何获取图像的元信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有图像节点
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

显示如何添加带有标签的新图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);

// 加载一张图片
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// 在文档节点中插入图片
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// 添加大纲元素节点
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

演示如何将图像从文件添加到具有用户定义属性的文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 从流中加载文档。
Document doc = new Document(dataDir + "Aspose.one");

// 获取文档的第一页。
Aspose.Note.Page page = doc.FirstChild;

// 从文件中加载图像。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 根据您的需要更改图像的大小（可选）。
                              Width = 100,
                              Height = 100,

                              // 设置图片在页面中的位置（可选）。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 设置图像对齐
                              Alignment = HorizontalAlignment.Right
                          };

// 将图像添加到页面。
page.AppendChildLast(image);
```

演示如何将图像从流添加到文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // 使用图像名称、扩展名和流加载第二张图像。
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 设置图像对齐
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

显示如何将图像从文件添加到文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 Outline 类对象并设置偏移属性
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);

// 通过文件路径加载图片。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 设置图像对齐
                              Alignment = HorizontalAlignment.Right
                          };

// 添加图片
outlineElem.AppendChildLast(image);

// 添加轮廓元素
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### 也可以看看

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
