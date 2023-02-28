---
title: Image.HorizontalOffset
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 수평 오프셋을 가져오거나 설정합니다.
type: docs
weight: 100
url: /ko/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

수평 오프셋을 가져오거나 설정합니다.

```csharp
public float HorizontalOffset { get; set; }
```

### 예

사용자 정의 속성을 사용하여 파일의 이미지를 문서에 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 스트림에서 문서를 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

// 문서의 첫 번째 페이지를 가져옵니다.
Aspose.Note.Page page = doc.FirstChild;

// 파일에서 이미지를 로드합니다.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 필요에 따라 이미지 크기를 변경합니다(선택 사항).
                              Width = 100,
                              Height = 100,

                              // 페이지에서 이미지의 위치를 설정합니다(선택 사항).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 이미지 정렬 설정
                              Alignment = HorizontalAlignment.Right
                          };

// 페이지에 이미지를 추가합니다.
page.AppendChildLast(image);
```

### 또한보십시오

* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


