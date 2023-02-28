---
title: Image.HyperlinkUrl
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 이미지와 연결된 하이퍼링크를 가져오거나 설정합니다.
type: docs
weight: 110
url: /ko/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

이미지와 연결된 하이퍼링크를 가져오거나 설정합니다.

```csharp
public string HyperlinkUrl { get; set; }
```

### 예

이미지에 하이퍼링크를 바인딩하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### 또한보십시오

* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


