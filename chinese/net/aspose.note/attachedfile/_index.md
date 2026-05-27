---
title: "类 AttachedFile"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.AttachedFile 类。表示一个附加文件"
type: docs
weight: 10
url: /zh/net/aspose.note/attachedfile/
---
## AttachedFile class

表示一个附加文件。

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile](attachedfile/#constructor_1)(string) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile](attachedfile/#constructor_2)(string, Stream) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile](attachedfile/#constructor_3)(string, Stream, ImageFormat) | 初始化 `AttachedFile` 类的新实例。 |
| [AttachedFile](attachedfile/#constructor_4)(string, Stream, Stream, ImageFormat) | 初始化 `AttachedFile` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | 获取或设置对齐方式。 |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | 获取或设置附件文件图标的正文替代文本。 |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | 获取或设置附件文件图标的标题替代文本。 |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | 获取嵌入文件的二进制数据。 |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | 获取嵌入文件的扩展名。 |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | 获取嵌入文件的名称。 |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | 获取原始文件的路径。 |
| [Height](../../aspose.note/attachedfile/height/) { get; } | 获取嵌入文件图标的原始高度。 |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | 获取或设置水平偏移。 |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | 获取与嵌入文件关联的图标的二进制数据。 |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | 获取图标的扩展名。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 获取一个值，指示此节点是否为复合节点。如果为 true，则该节点可以拥有子节点。 |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | 获取或设置一个值，指示文件的视图是否为打印输出。 |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | 获取或设置一个值，指示图标大小的值是否已被用户显式更新。 |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | 获取或设置最后修改时间。 |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | 获取或设置显示嵌入文件图标的最大高度。 |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | 获取或设置显示嵌入文件图标的最大宽度。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [ParsingErrorInfo](../../aspose.note/attachedfile/parsingerrorinfo/) { get; } | 获取访问文件时发生的错误数据。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | 获取段落的所有标签列表。 |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | 获取或设置嵌入文件的文本表示。该字符串不得包含值为10（换行）或13（回车）的任何字符。 |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | 获取或设置垂直偏移量。 |
| [Width](../../aspose.note/attachedfile/width/) { get; } | 获取嵌入文件图标的原始宽度。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | 接受节点的访问者。 |

## 示例

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

### 另请参阅

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


