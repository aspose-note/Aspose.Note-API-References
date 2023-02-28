---
title: Image.Width
second_title: Aspose.Note for .NET API 参考
description: Image 财产. 获取或设置宽度这是MS OneNote文档中图片的真实宽度
type: docs
weight: 180
url: /zh/net/aspose.note/image/width/
---
## Image.Width property

获取或设置宽度。这是MS OneNote文档中图片的真实宽度。

```csharp
public float Width { get; set; }
```

### 例子

显示如何获取图像的元信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有Image节点
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


