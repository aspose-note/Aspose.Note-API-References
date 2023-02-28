---
title: Class TextStyle
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.TextStyle 수업. 텍스트 스타일을 지정합니다.
type: docs
weight: 970
url: /ko/net/aspose.note/textstyle/
---
## TextStyle class

텍스트 스타일을 지정합니다.

```csharp
public sealed class TextStyle : Style
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TextStyle](textstyle/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | "en-US" 문화권으로 스타일을 가져옵니다. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | MS OneNote에서 제목 날짜의 기본 스타일을 가져옵니다. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | MS OneNote에서 제목 텍스트의 기본 스타일을 가져옵니다. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | MS OneNote에서 제목 시간의 기본 스타일을 가져옵니다. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | 글꼴 색상을 가져오거나 설정합니다. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | 글꼴 이름을 가져오거나 설정합니다. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | 글꼴 크기를 가져오거나 설정합니다. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | 글꼴 스타일을 가져옵니다. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | 하이라이트 색상을 가져오거나 설정합니다. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | 하이퍼링크 주소를 가져오거나 설정합니다. 값이 다음과 같은 경우 설정해야 합니다.[`IsHyperlink`](./ishyperlink/) 속성은 true입니다. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | 텍스트 스타일이 굵게 표시되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | 텍스트 스타일이 숨겨져 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | 텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | 텍스트 스타일이 기울임꼴인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | 텍스트 스타일이 수학 형식인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | 텍스트 스타일이 취소선인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | 텍스트 스타일이 아래 첨자인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | 텍스트 스타일이 위 첨자인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | 텍스트 스타일이 밑줄인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | 텍스트의 언어를 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | 유형에 대한 해시 함수 역할을 합니다. |

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

텍스트의 교정 언어를 설정합니다.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

* class [Style](../style/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


