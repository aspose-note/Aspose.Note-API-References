---
title: "Page.BackgroundColor"
second_title: "Aspose.Note for .NET API 参考"
description: "Page 属性。获取或设置页面的背景颜色"
type: docs
weight: 30
url: /zh/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

获取或设置页面的背景颜色。

```csharp
public Color BackgroundColor { get; set; }
```

## 示例

展示如何设置页面的背景颜色。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子项
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

展示如何对文档应用暗色主题样式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### 另请参阅

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


