---
title: Image.VerticalOffset
second_title: Aspose.Note for .NET API 参考
description: Image 财产. 获取或设置垂直偏移量
type: docs
weight: 170
url: /zh/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

获取或设置垂直偏移量。

```csharp
public float VerticalOffset { get; set; }
```

### 例子

显示如何将图像从文件添加到具有用户定义属性的文档。

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
                              // 根据需要更改图像的大小（可选）。
                              Width = 100,
                              Height = 100,

                              // 设置图像在页面中的位置（可选）。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 设置图像对齐
                              Alignment = HorizontalAlignment.Right
                          };

// 将图像添加到页面。
page.AppendChildLast(image);
```

### 也可以看看

* class [Image](../)
* 命名空间 [Aspose.Note](../../image/)
* 部件 [Aspose.Note](../../../)


