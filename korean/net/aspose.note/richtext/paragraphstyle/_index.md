---
title: RichText.ParagraphStyle
second_title: .NET API 참조용 Aspose.Note
description: RichText 재산. 단락 스타일을 가져오거나 설정합니다. 이 설정은 일치하는 TextStyle 객체가 없는 경우에 사용됩니다.Styles 컬렉션 또는 이 개체가 필요한 설정을 지정하지 않습니다.
type: docs
weight: 60
url: /ko/net/aspose.note/richtext/paragraphstyle/
---
## RichText.ParagraphStyle property

단락 스타일을 가져오거나 설정합니다. 이 설정은 일치하는 TextStyle 객체가 없는 경우에 사용됩니다.Styles 컬렉션 또는 이 개체가 필요한 설정을 지정하지 않습니다.

```csharp
public ParagraphStyle ParagraphStyle { get; set; }
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

페이지의 제목을 설정하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

단락 스타일을 사용하여 텍스트 형식으로 조작합니다.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

태그가 있는 새 단락을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// 텍스트 노드 추가
outlineElem.AppendChildLast(text);

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

태그 세부 정보에 액세스하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "TagFile.one");

// 모든 RichText 노드 가져오기
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 각 노드를 통해 반복
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 속성 검색
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

중국어 번호 매기기로 새 목록을 삽입하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote 문서 초기화
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote 페이지 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 텍스트 스타일 설정 적용
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 같은 아웃라인의 숫자는 자동으로 증가합니다.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

새 글머리 기호 목록을 삽입하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document 클래스의 객체 생성
Aspose.Note.Document doc = new Aspose.Note.Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// TextStyle 클래스 개체를 초기화하고 서식 지정 속성을 설정합니다.
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement 클래스 개체를 초기화하고 글머리 기호를 적용합니다.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText 클래스 객체 초기화 및 텍스트 스타일 적용
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 아웃라인 노드 추가
page.AppendChildLast(outline);
// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

번호가 매겨진 새 목록을 삽입하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// TextStyle 클래스 개체를 초기화하고 서식 지정 속성을 설정합니다.
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement 클래스 객체 초기화 및 번호 매기기 적용
// 같은 아웃라인의 숫자는 자동으로 증가합니다.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

주간 회의를 위한 템플릿을 준비하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// Document 클래스의 객체 생성
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
```

하이퍼링크를 텍스트에 바인딩하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tasks();

// Document 클래스의 객체 생성
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem);

// Title 클래스 객체 초기화
Title title = new Title() { TitleText = titleText };

// 페이지 클래스 객체 초기화
Page page = new Note.Page() { Title = title };

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### 또한보십시오

* class [ParagraphStyle](../../paragraphstyle/)
* class [RichText](../)
* 네임스페이스 [Aspose.Note](../../richtext/)
* 집회 [Aspose.Note](../../../)


