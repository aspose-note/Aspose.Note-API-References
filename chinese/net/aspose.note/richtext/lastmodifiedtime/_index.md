---
title: "RichText.LastModifiedTime"
second_title: "Aspose.Note for .NET API 参考"
description: "RichText 属性。获取或设置最后修改时间"
type: docs
weight: 60
url: /zh/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

获取或设置最后修改时间。

```csharp
public DateTime LastModifiedTime { get; set; }
```

## 示例

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

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


