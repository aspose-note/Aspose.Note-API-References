---
title: Image.AlternativeTextDescription
second_title: Aspose.Note for .NET API 参考
description: Image 财产. 获取或设置正文图像的替代文本
type: docs
weight: 30
url: /zh/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

获取或设置正文图像的替代文本。

```csharp
public string AlternativeTextDescription { get; set; }
```

### 例子

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

### 也可以看看

* class [Image](../)
* 命名空间 [Aspose.Note](../../image/)
* 部件 [Aspose.Note](../../../)


