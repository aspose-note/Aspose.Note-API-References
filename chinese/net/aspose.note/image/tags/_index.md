---
title: "Image.Tags"
second_title: "Aspose.Note for .NET API 参考"
description: "Image 属性。获取段落的所有标签列表。"
type: docs
weight: 160
url: /zh/net/aspose.note/image/tags/
---
## Image.Tags property

获取段落的所有标签列表。

```csharp
public List<ITag> Tags { get; }
```

## 示例

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

### 另请参阅

* interface [ITag](../../itag/)
* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


