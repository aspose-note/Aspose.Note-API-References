---
title: Page.BackgroundColor
second_title: .NET API 참조용 Aspose.Note
description: Page 재산. 페이지의 배경색을 가져오거나 설정합니다.
type: docs
weight: 30
url: /ko/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

페이지의 배경색을 가져오거나 설정합니다.

```csharp
public Color BackgroundColor { get; set; }
```

### 예

페이지의 배경색을 설정하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

어두운 테마 스타일을 문서에 적용하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
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

### 또한보십시오

* class [Page](../)
* 네임스페이스 [Aspose.Note](../../page/)
* 집회 [Aspose.Note](../../../)


