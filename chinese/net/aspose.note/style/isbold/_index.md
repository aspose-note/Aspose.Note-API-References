---
title: "Style.IsBold"
second_title: "Aspose.Note for .NET API 参考"
description: "Style 属性。获取或设置一个值，指示文本样式是否为粗体"
type: docs
weight: 60
url: /zh/net/aspose.note/style/isbold/
---
## Style.IsBold property

获取或设置一个值，指示文本样式是否为粗体。

```csharp
public bool IsBold { get; set; }
```

## 示例

让我们通过增大字体大小来强调页面的标题，而不是其他标题。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Aspose.one");

// 遍历页面的标题。
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

让我们通过高亮来强调最新文本的更改。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Aspose.one");

// 获取上周修改的 RichText 节点。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // 设置高亮颜色
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // 设置高亮颜色
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### 另请参阅

* class [Style](../)
* namespace [Aspose.Note](../../style/)
* assembly [Aspose.Note](../../../)


