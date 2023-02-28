---
title: Class Outline
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Outline 수업. 는 개요를 나타냅니다.
type: docs
weight: 450
url: /ko/net/aspose.note/outline/
---
## Outline class

는 개요를 나타냅니다.

```csharp
public sealed class Outline : IndentatedNode<IOutlineChildNode>, IPageChildNode
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Outline](outline/#constructor)() | 의 새 인스턴스를 초기화합니다.`Outline` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved/) { get; set; } | 외곽선의 하위 항목을 이동할 수 있는지 여부를 가져옵니다. |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset/) { get; set; } | 수평 오프셋을 가져오거나 설정합니다. |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [MaxHeight](../../aspose.note/outline/maxheight/) { get; set; } | 최대 높이를 가져오거나 설정합니다. |
| [MaxWidth](../../aspose.note/outline/maxwidth/) { get; set; } | 최대 너비를 가져오거나 설정합니다. |
| [MinWidth](../../aspose.note/outline/minwidth/) { get; set; } | 최소 너비를 가져오거나 설정합니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |
| [ReservedWidth](../../aspose.note/outline/reservedwidth/) { get; set; } | 예약된 너비를 가져오거나 설정합니다. |
| [VerticalOffset](../../aspose.note/outline/verticaloffset/) { get; set; } | 수직 오프셋을 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### 예

태그로 새 이미지를 추가하는 방법을 보여줍니다.

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

// 이미지 로드
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// 문서 노드에 이미지 삽입
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
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

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


