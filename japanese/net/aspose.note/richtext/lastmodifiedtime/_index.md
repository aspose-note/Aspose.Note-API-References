---
title: RichText.LastModifiedTime
second_title: Aspose.Note for .NET API リファレンス
description: RichText 財産. 最終変更時刻を取得または設定します
type: docs
weight: 30
url: /ja/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

最終変更時刻を取得または設定します。

```csharp
public DateTime LastModifiedTime { get; set; }
```

### 例

ハイライトで最新のテキストの変更点を強調しましょう。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Aspose.one");

// 先週変更された RichText ノードを取得します。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // ハイライトの色を設定
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // ハイライトの色を設定
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### 関連項目

* class [RichText](../)
* 名前空間 [Aspose.Note](../../richtext/)
* 組み立て [Aspose.Note](../../../)


