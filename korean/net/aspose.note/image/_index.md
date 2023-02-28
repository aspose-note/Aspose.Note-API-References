---
title: Class Image
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Image 수업. 이미지를 나타냅니다.
type: docs
weight: 250
url: /ko/net/aspose.note/image/
---
## Image class

이미지를 나타냅니다.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Image](image/#constructor)() | 의 새 인스턴스를 초기화합니다.`Image` 클래스. |
| [Image](image/#constructor_4)(string, Stream) | 의 새 인스턴스를 초기화합니다.`Image` 클래스. |
| [Image](image/#constructor_5)(string, string, string) | 의 새 인스턴스를 초기화합니다.`Image` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | 정렬을 가져오거나 설정합니다. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | 이미지의 대체 텍스트 본문을 가져오거나 설정합니다. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | 이미지의 대체 텍스트 제목을 가져오거나 설정합니다. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | 이미지 데이터 저장소를 가져옵니다. |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [FileName](../../aspose.note/image/filename/) { get; } | 파일 이름을 가져옵니다. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | 이미지 파일의 경로를 가져옵니다. |
| [Format](../../aspose.note/image/format/) { get; } | 이미지 형식을 가져옵니다. |
| [Height](../../aspose.note/image/height/) { get; set; } | 높이를 가져오거나 설정합니다. 이것은 MS OneNote 문서에 있는 이미지의 실제 높이입니다. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | 수평 오프셋을 가져오거나 설정합니다. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | 이미지와 연결된 하이퍼링크를 가져오거나 설정합니다. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | 이미지가 배경 이미지인지 여부를 가져옵니다. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 이 노드가 복합인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드에 하위 노드가 있을 수 있습니다. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | 원래 높이를 가져옵니다. 크기를 조정하기 전 이미지의 원래 너비입니다. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | 원래 너비를 가져옵니다. 크기를 조정하기 전 이미지의 원래 너비입니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |
| [Tags](../../aspose.note/image/tags/) { get; } | 단락의 모든 태그 목록을 가져옵니다. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | 수직 오프셋을 가져오거나 설정합니다. |
| [Width](../../aspose.note/image/width/) { get; set; } | 너비를 가져오거나 설정합니다. MS OneNote 문서에 있는 이미지의 실제 너비입니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |

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

문서에서 이미지를 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Images();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 이미지 노드 가져오기
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 이미지 바이트를 파일에 저장
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

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

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


