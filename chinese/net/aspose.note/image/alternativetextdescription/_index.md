---
title: "Image.AlternativeTextDescription"
second_title: "Aspose.Note for .NET API 参考"
description: "Image 属性。获取或设置图像的替代文本正文。"
type: docs
weight: 30
url: /zh/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

获取或设置图像的正文替代文本。

```csharp
public string AlternativeTextDescription { get; set; }
```

## 示例

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

### 另请参阅

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


