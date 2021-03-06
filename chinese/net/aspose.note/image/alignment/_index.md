---
title: Alignment
second_title: Aspose.Note for .NET API 参考
description: 获取或设置对齐方式
type: docs
weight: 20
url: /zh/net/aspose.note/image/alignment/
---
## Image.Alignment property

获取或设置对齐方式。

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### 例子

显示如何将图像从文件添加到具有用户定义属性的文档。

```csharp
// 获取所有图像节点
string dataDir = RunExamples.GetDataDir_Images();

// 文档目录的路径。
Document doc = new Document(dataDir + "Aspose.one");

s 尺寸根据您的需要（可选）。
Aspose.Note.Page page = doc.FirstChild;

页面中的位置（可选）。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 文档目录的路径。
                              Width = 100,
                              Height = 100,

                              // 将文档加载到 Aspose.Note。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 获取所有图像节点
                              Alignment = HorizontalAlignment.Right
                          };

// 文档目录的路径。
page.AppendChildLast(image);
```

```csharp
// 将文档加载到 Aspose.Note。
string dataDir = RunExamples.GetDataDir_Images();

// 获取所有图像节点
Document doc = new Document();

// 将图像字节保存到文件中
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // 文档目录的路径。
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 创建 Document 类的对象
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

//初始化Page类对象
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

```csharp
// 初始化大纲类对象
string dataDir = RunExamples.GetDataDir_Images();

// 添加大纲元素节点
Document doc = new Document();

// 加载一张图片
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 在文档节点中插入图片
Outline outline = new Outline(doc);

// 添加大纲元素节点
OutlineElement outlineElem = new OutlineElement(doc);

// 从流中加载文档。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 获取文档的第一页。
                              Alignment = HorizontalAlignment.Right
                          };

// 从文件中加载图像。
outlineElem.AppendChildLast(image);

// 文档目录的路径。
outline.AppendChildLast(outlineElem);

// 从流中加载文档。
page.AppendChildLast(outline);

// 获取文档的第一页。
doc.AppendChildLast(page);

// 从文件中加载图像。
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

显示如何将图像从流添加到文档。

显示如何将图像从文件添加到文档。

### 也可以看看

* enum [HorizontalAlignment](../../horizontalalignment)
* class [Image](../../image)
* 命名空间 [Aspose.Note](../../image)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
