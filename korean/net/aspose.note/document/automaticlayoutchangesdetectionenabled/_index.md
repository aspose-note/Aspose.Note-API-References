---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: .NET API 참조용 Aspose.Note
description: Document 재산. Aspose.Note가 레이아웃 변경을 자동으로 감지하는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은진실 .
type: docs
weight: 20
url: /ko/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Aspose.Note가 레이아웃 변경을 자동으로 감지하는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본값은`진실` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### 예

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

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


