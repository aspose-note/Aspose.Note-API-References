---
title: Style.Highlight
second_title: .NET API 참조용 Aspose.Note
description: Style 재산. 하이라이트 색상을 가져오거나 설정합니다.
type: docs
weight: 50
url: /ko/net/aspose.note/style/highlight/
---
## Style.Highlight property

하이라이트 색상을 가져오거나 설정합니다.

```csharp
public Color Highlight { get; set; }
```

### 예

텍스트의 스타일을 변경하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 문서를 Aspose.Note에 로드합니다.
Document document = new Document(dataDir + "Aspose.one");

// 특정 RichText 노드 가져오기
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // 글꼴 색상 설정
    run.Style.FontColor = Color.Yellow;

    // 강조 색상 설정
    run.Style.Highlight = Color.Blue;

    // 글꼴 크기 설정
    run.Style.FontSize = 20;
}
```

다양한 스타일의 텍스트가 포함된 테이블을 구성하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// 테이블 앞의 요약 텍스트
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// 열 세트와 헤더 행을 추가합시다.
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// 5개의 빈 행이 있습니다. 행의 배경색이 서로 바뀝니다.
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// '연락처' 열의 콘텐츠에 대한 템플릿을 추가해 보겠습니다.
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

### 또한보십시오

* class [Style](../)
* 네임스페이스 [Aspose.Note](../../style/)
* 집회 [Aspose.Note](../../../)


