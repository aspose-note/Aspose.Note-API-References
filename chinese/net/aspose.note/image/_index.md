---
title: "类 Image"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Image 类。表示一个图像"
type: docs
weight: 250
url: /zh/net/aspose.note/image/
---
## Image class

表示一个图像。

```csharp
public sealed class Image : CompositeNode<Loop>, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Image](image/#constructor)() | 初始化 `Image` 类的新实例。 |
| [Image](image/#constructor_1)(string) | 初始化 `Image` 类的新实例。 |
| [Image](image/#constructor_2)(string, Stream) | 初始化 `Image` 类的新实例。 |
| [Image](image/#constructor_3)(string, string, string) | 初始化 `Image` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | 获取或设置对齐方式。 |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | 获取或设置图像的正文替代文本。 |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | 获取或设置图像的替代文本标题。 |
| [Bytes](../../aspose.note/image/bytes/) { get; } | 获取图像数据存储。 |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [FileName](../../aspose.note/image/filename/) { get; } | 获取文件名。 |
| [FilePath](../../aspose.note/image/filepath/) { get; } | 获取图像文件的路径。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Format](../../aspose.note/image/format/) { get; } | 获取图像的格式。 |
| [Height](../../aspose.note/image/height/) { get; set; } | 获取或设置高度。这是图像在 MS OneNote 文档中的实际高度。 |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | 获取或设置水平偏移。 |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | 获取或设置与图像关联的超链接。 |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | 获取图像是否为背景图像。 |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | 获取或设置最后修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | 获取原始高度。这是图像在调整大小之前的原始宽度。 |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | 获取原始宽度。这是图像在调整大小之前的原始宽度。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |
| [Tags](../../aspose.note/image/tags/) { get; } | 获取段落的所有标签列表。 |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | 获取或设置垂直偏移量。 |
| [Width](../../aspose.note/image/width/) { get; set; } | 获取或设置宽度。这是图像在 MS OneNote 文档中的实际宽度。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Loop&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Loop[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Replace](../../aspose.note/image/replace/)(Image) | 用提供的 Image 对象的数据替换当前图像数据。 |

## 示例

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

展示如何添加带标签的新图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();

// 加载图像
Image image = new Image(dataDir + "icon.jpg");

// 在文档节点中插入图像
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

### 另请参阅

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Loop](../loop/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


