---
title: Class Title
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Title 수업. 제목을 나타냅니다.
type: docs
weight: 980
url: /ko/net/aspose.note/title/
---
## Title class

제목을 나타냅니다.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Title](title/#constructor)() | 의 새 인스턴스를 초기화합니다.`Title` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset/) { get; set; } | 수평 오프셋을 가져오거나 설정합니다. |
| override [IsComposite](../../aspose.note/title/iscomposite/) { get; } | 이 노드가 복합인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드에 하위 노드가 있을 수 있습니다. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |
| [TitleDate](../../aspose.note/title/titledate/) { get; set; } | 제목에 있는 날짜의 문자열 표현을 가져오거나 설정합니다. |
| [TitleText](../../aspose.note/title/titletext/) { get; set; } | 제목의 텍스트를 가져오거나 설정합니다. |
| [TitleTime](../../aspose.note/title/titletime/) { get; set; } | 제목에 있는 시간의 문자열 표현을 가져오거나 설정합니다. |
| [VerticalOffset](../../aspose.note/title/verticaloffset/) { get; set; } | 수직 오프셋을 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/title/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes/#getchildnodes_1)() | 노드 유형별로 모든 하위 노드를 가져옵니다. |
| [GetEnumerator](../../aspose.note/title/getenumerator/)() | 의 자식 노드를 반복하는 열거자를 반환합니다.`Title` . |

### 예

페이지 기록을 편집하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서를 로드하고 첫 번째 자식 가져오기           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

문서를 만들고 기본 옵션을 사용하여 html 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote 문서 초기화
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// HTML 형식으로 저장
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

문서를 생성하고 지정된 페이지 범위를 html 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote 문서 초기화
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML 형식으로 저장
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

제목 페이지가 있는 문서를 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document 클래스의 객체 생성
Document doc = new Aspose.Note.Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 페이지 제목 속성 설정
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 문서에 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

다양한 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 새 문서 초기화
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 새 페이지 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 문서의 모든 텍스트에 대한 기본 스타일입니다.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서를 다른 형식으로 저장하고, 텍스트 글꼴 크기를 설정하고, 레이아웃 변경을 수동으로 감지합니다.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### 또한보십시오

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* class [RichText](../richtext/)
* interface [IPageChildNode](../ipagechildnode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


