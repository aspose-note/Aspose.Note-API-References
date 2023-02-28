---
title: Image.Tags
second_title: .NET API 참조용 Aspose.Note
description: Image 재산. 단락의 모든 태그 목록을 가져옵니다.
type: docs
weight: 160
url: /ko/net/aspose.note/image/tags/
---
## Image.Tags property

단락의 모든 태그 목록을 가져옵니다.

```csharp
public List<ITag> Tags { get; }
```

### 예

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

### 또한보십시오

* interface [ITag](../../itag/)
* class [Image](../)
* 네임스페이스 [Aspose.Note](../../image/)
* 집회 [Aspose.Note](../../../)


