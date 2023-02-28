---
title: TextStyle.IsHyperlink
second_title: .NET API 참조용 Aspose.Note
description: TextStyle 재산. 텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 가져오거나 설정합니다.
type: docs
weight: 80
url: /ko/net/aspose.note/textstyle/ishyperlink/
---
## TextStyle.IsHyperlink property

텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IsHyperlink { get; set; }
```

### 예

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

* class [TextStyle](../)
* 네임스페이스 [Aspose.Note](../../textstyle/)
* 집회 [Aspose.Note](../../../)


