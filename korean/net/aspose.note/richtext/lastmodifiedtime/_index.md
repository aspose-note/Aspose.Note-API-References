---
title: RichText.LastModifiedTime
second_title: .NET API 참조용 Aspose.Note
description: RichText 재산. 마지막 수정 시간을 가져오거나 설정합니다.
type: docs
weight: 30
url: /ko/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

마지막 수정 시간을 가져오거나 설정합니다.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### 예

강조 표시를 통해 최신 텍스트의 변경 사항을 강조해 봅시다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Aspose.one");

// 지난주에 수정된 RichText 노드를 가져옵니다.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // 강조 색상 설정
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // 강조 색상 설정
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### 또한보십시오

* class [RichText](../)
* 네임스페이스 [Aspose.Note](../../richtext/)
* 집회 [Aspose.Note](../../../)


