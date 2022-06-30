---
title: AttachedFile
second_title: Aspose.Note for .NET API 参考
description: 表示附加文件
type: docs
weight: 10
url: /zh/net/aspose.note/attachedfile/
---
## AttachedFile class

表示附加文件。

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [AttachedFile](attachedfile#constructor)() | 初始化[`AttachedFile`](../attachedfile)类的新实例。 |
| [AttachedFile](attachedfile#constructor_6)(string, Stream) | 初始化[`AttachedFile`](../attachedfile)类的新实例。 |
| [AttachedFile](attachedfile#constructor_7)(string, Stream, ImageFormat) | 初始化[`AttachedFile`](../attachedfile)类的新实例。 |
| [AttachedFile](attachedfile#constructor_8)(string, Stream, Stream, ImageFormat) | 初始化[`AttachedFile`](../attachedfile)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment) { get; set; } | 获取或设置对齐方式。 |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription) { get; set; } | 获取或设置正文的附加文件图标的替代文本。 |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle) { get; set; } | 获取或设置附件图标的替代文本标题。 |
| [Bytes](../../aspose.note/attachedfile/bytes) { get; } | 获取嵌入文件的二进制数据。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [Extension](../../aspose.note/attachedfile/extension) { get; } | 获取嵌入文件的扩展名。 |
| [FileName](../../aspose.note/attachedfile/filename) { get; } | 获取嵌入文件的名称。 |
| [FilePath](../../aspose.note/attachedfile/filepath) { get; } | 获取原始文件的路径。 |
| [Height](../../aspose.note/attachedfile/height) { get; } | 获取嵌入文件图标的原始高度。 |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset) { get; set; } | 获取或设置水平偏移。 |
| [Icon](../../aspose.note/attachedfile/icon) { get; } | 获取与嵌入文件关联的图标的二进制数据。 |
| [IconExtension](../../aspose.note/attachedfile/iconextension) { get; } | 获取图标的扩展名。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | 获取一个值，该值指示此节点是否为复合节点。如果为 true，则该节点可以有子节点。 |
| [IsPrintout](../../aspose.note/attachedfile/isprintout) { get; set; } | 获取或设置一个值，该值指示文件的视图是否为打印输出。 |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser) { get; set; } | 获取或设置一个值，该值指示图标大小的值是否由用户显式更新。 |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime) { get; set; } | 获取或设置最后修改时间。 |
| [MaxHeight](../../aspose.note/attachedfile/maxheight) { get; set; } | 获取或设置显示嵌入文件图标的最大高度。 |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth) { get; set; } | 获取或设置显示嵌入文件图标的最大宽度。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [Tags](../../aspose.note/attachedfile/tags) { get; } | 获取段落所有标签的列表。 |
| [Text](../../aspose.note/attachedfile/text) { get; set; } | 获取或设置嵌入文件的文本表示。字符串不得包含任何值为 10（换行）或 13（回车）的字符。 |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset) { get; set; } | 获取或设置垂直偏移量。 |
| [Width](../../aspose.note/attachedfile/width) { get; } | 获取嵌入文件图标的原始宽度。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept)(DocumentVisitor) | 接受节点的访问者。 |

### 例子

显示如何获取附件的内容。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Sample1.one");

// 获取附件节点列表
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// 遍历所有节点
foreach (AttachedFile file in nodes)
{
    // 将附件加载到流对象
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

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);

// 初始化 AttachedFile 类对象
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// 添加附件
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

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // 初始化 AttachedFile 类对象并传递其图标路径
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 添加附件
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

显示如何使用文件路径将文件添加到文档中。

显示如何将文件从流添加到文档。

### 也可以看看

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
