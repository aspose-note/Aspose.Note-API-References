---
title: "Image.HorizontalOffset"
second_title: "Aspose.Note for .NET API 参考"
description: "Image 属性。获取或设置水平偏移"
type: docs
weight: 100
url: /zh/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

获取或设置水平偏移。

```csharp
public float HorizontalOffset { get; set; }
```

## 示例

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

### 另请参阅

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


