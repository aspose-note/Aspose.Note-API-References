---
title: Class ParagraphStyle
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.ParagraphStyle 수업. 일치하는 TextStyle 객체가 없는 경우 사용할 텍스트 스타일 설정Styles 컬렉션 또는 이 개체가 필요한 설정을 지정하지 않습니다.
type: docs
weight: 510
url: /ko/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

일치하는 TextStyle 객체가 없는 경우 사용할 텍스트 스타일 설정Styles 컬렉션 또는 이 개체가 필요한 설정을 지정하지 않습니다.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | 의 새 인스턴스를 초기화합니다.`ParagraphStyle` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | 기본 설정으로 ParagraphStyle을 가져옵니다. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | 글꼴 색상을 가져오거나 설정합니다. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | 글꼴 이름을 가져오거나 설정합니다. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | 글꼴 크기를 가져오거나 설정합니다. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | 글꼴 스타일을 가져옵니다. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | 하이라이트 색상을 가져오거나 설정합니다. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | 텍스트 스타일이 굵게 표시되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | 텍스트 스타일이 기울임꼴인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | 텍스트 스타일이 취소선인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | 텍스트 스타일이 아래 첨자인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | 텍스트 스타일이 위 첨자인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | 텍스트 스타일이 밑줄인지 여부를 나타내는 값을 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | 유형에 대한 해시 함수 역할을 합니다. |

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

### 또한보십시오

* class [Style](../style/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


