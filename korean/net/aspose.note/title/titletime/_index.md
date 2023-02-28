---
title: Title.TitleTime
second_title: .NET API 참조용 Aspose.Note
description: Title 재산. 제목에 있는 시간의 문자열 표현을 가져오거나 설정합니다.
type: docs
weight: 70
url: /ko/net/aspose.note/title/titletime/
---
## Title.TitleTime property

제목에 있는 시간의 문자열 표현을 가져오거나 설정합니다.

```csharp
public RichText TitleTime { get; set; }
```

### 예

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

* class [RichText](../../richtext/)
* class [Title](../)
* 네임스페이스 [Aspose.Note](../../title/)
* 집회 [Aspose.Note](../../../)


