---
title: Image.Height
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 높이를 가져오거나 설정합니다. 이것은 MS OneNote 문서에 있는 이미지의 실제 높이입니다.
type: docs
weight: 90
url: /ko/net/aspose.note/image/height/
---
## Image.Height property

높이를 가져오거나 설정합니다. 이것은 MS OneNote 문서에 있는 이미지의 실제 높이입니다.

```csharp
public float Height { get; set; }
```

### 예

이미지의 메타 정보를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 이미지 노드 가져오기
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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


