---
title: Image.Alignment
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 정렬을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note/image/alignment/
---
## Image.Alignment property

정렬을 가져오거나 설정합니다.

```csharp
public HorizontalAlignment Alignment { get; set; }
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

스트림에서 문서로 이미지를 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // 이미지 이름, 확장자 및 스트림을 사용하여 두 번째 이미지를 로드합니다.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 이미지 정렬 설정
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

파일에서 문서로 이미지를 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline 클래스 객체 초기화 및 오프셋 속성 설정
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

// 파일 경로로 이미지를 로드합니다.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 이미지 정렬 설정
                              Alignment = HorizontalAlignment.Right
                          };

// 이미지 추가
outlineElem.AppendChildLast(image);

// 아웃라인 요소 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

// OneNote 문서 저장
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### 또한보십시오

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


