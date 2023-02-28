---
title: Style.IsBold
second_title: .NET API 참조용 Aspose.Note
description: Style 재산. 텍스트 스타일이 굵게 표시되는지 여부를 나타내는 값을 가져오거나 설정합니다.
type: docs
weight: 60
url: /ko/net/aspose.note/style/isbold/
---
## Style.IsBold property

텍스트 스타일이 굵게 표시되는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IsBold { get; set; }
```

### 예

글꼴 크기를 늘려 다른 헤더 중에서 페이지의 제목을 강조해 봅시다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Aspose.one");

// 페이지 제목을 반복합니다.
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

* class [Style](../)
* 네임스페이스 [Aspose.Note](../../style/)
* 집회 [Aspose.Note](../../../)


