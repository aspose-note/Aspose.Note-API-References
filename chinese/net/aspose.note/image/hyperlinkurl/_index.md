---
title: Image.HyperlinkUrl
second_title: Aspose.Note for .NET API 参考
description: Image 财产. 获取或设置与图像关联的超链接
type: docs
weight: 110
url: /zh/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

获取或设置与图像关联的超链接。

```csharp
public string HyperlinkUrl { get; set; }
```

### 例子

显示如何将超链接绑定到图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### 也可以看看

* class [Image](../)
* 命名空间 [Aspose.Note](../../image/)
* 部件 [Aspose.Note](../../../)


