---
title: Image.AlternativeTextDescription
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 이미지의 대체 텍스트 본문을 가져오거나 설정합니다.
type: docs
weight: 30
url: /ko/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

이미지의 대체 텍스트 본문을 가져오거나 설정합니다.

```csharp
public string AlternativeTextDescription { get; set; }
```

### 예

이미지에 대한 텍스트 설명을 설정하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

### 또한보십시오

* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


