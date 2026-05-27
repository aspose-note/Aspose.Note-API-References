---
title: "Image.HyperlinkUrl"
second_title: "Aspose.Note for .NET API 参考"
description: "Image 属性。获取或设置与图像关联的超链接"
type: docs
weight: 110
url: /zh/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

获取或设置与图像关联的超链接。

```csharp
public string HyperlinkUrl { get; set; }
```

## 示例

展示如何将超链接绑定到图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page();

var image = new Image(dataDir + "image.jpg") { HyperlinkUrl = "https://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### 另请参阅

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


