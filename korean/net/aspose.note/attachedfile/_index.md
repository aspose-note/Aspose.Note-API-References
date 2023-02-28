---
title: Class AttachedFile
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.AttachedFile 수업. 첨부파일을 나타냅니다.
type: docs
weight: 10
url: /ko/net/aspose.note/attachedfile/
---
## AttachedFile class

첨부파일을 나타냅니다.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | 의 새 인스턴스를 초기화합니다.`AttachedFile` 클래스. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | 의 새 인스턴스를 초기화합니다.`AttachedFile` 클래스. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | 의 새 인스턴스를 초기화합니다.`AttachedFile` 클래스. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | 의 새 인스턴스를 초기화합니다.`AttachedFile` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | 정렬을 가져오거나 설정합니다. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | 첨부파일의 아이콘에 대한 대체 텍스트 본문을 가져오거나 설정합니다. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | 첨부파일 아이콘의 대체 텍스트 제목을 가져오거나 설정합니다. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | 포함된 파일의 이진 데이터를 가져옵니다. |
| [Document](../../aspose.note/node/document/) { get; } | 노드의 문서를 가져옵니다. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | 포함된 파일의 확장자를 가져옵니다. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | 포함된 파일의 이름을 가져옵니다. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | 원본 파일의 경로를 가져옵니다. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | 포함된 파일 아이콘의 원래 높이를 가져옵니다. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | 수평 오프셋을 가져오거나 설정합니다. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | 포함된 파일과 연결된 아이콘의 이진 데이터를 가져옵니다. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | 아이콘의 확장자를 가져옵니다. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 이 노드가 복합인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드에 하위 노드가 있을 수 있습니다. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | 파일 보기가 출력인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | 아이콘 크기 값이 사용자에 의해 명시적으로 업데이트되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | 마지막 수정 시간을 가져오거나 설정합니다. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | 포함된 파일 아이콘을 표시할 최대 높이를 가져오거나 설정합니다. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | 포함된 파일 아이콘을 표시할 최대 너비를 가져오거나 설정합니다. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 동일한 노드 트리 수준에서 다음 노드를 가져옵니다. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 노드 유형을 가져옵니다. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 상위 노드를 가져옵니다. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 동일한 노드 트리 수준에서 이전 노드를 가져옵니다. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | 단락의 모든 태그 목록을 가져옵니다. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | 포함된 파일의 텍스트 표현을 가져오거나 설정합니다. 문자열은 값 10(줄 바꿈) 또는 13(캐리지 리턴)의 문자를 포함하면 안 됩니다. |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | 수직 오프셋을 가져오거나 설정합니다. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | 포함된 파일 아이콘의 원래 너비를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | 노드의 방문자를 수락합니다. |

### 예

첨부 파일의 내용을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Sample1.one");

// 첨부 파일 노드 목록 가져오기
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// 모든 노드를 반복합니다.
foreach (AttachedFile file in nodes)
{
    // 첨부 파일을 스트림 객체에 로드
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // 로컬 파일 생성
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // 파일 스트림 복사
            CopyStream(outputStream, fileStream);
        }
    }
}
```

파일 경로를 사용하여 문서에 파일을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile 클래스 객체 초기화
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// 첨부파일 추가
outlineElem.AppendChildLast(attachedFile);

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

스트림에서 문서로 파일을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Attachments();

// Document 클래스의 객체 생성
Document doc = new Document();

// 페이지 클래스 객체 초기화
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 아웃라인 클래스 객체 초기화
Outline outline = new Outline(doc);

// OutlineElement 클래스 객체 초기화
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // AttachedFile 클래스 개체를 초기화하고 해당 아이콘 경로도 전달합니다.
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // 첨부파일 추가
    outlineElem.AppendChildLast(attachedFile);
}

// 아웃라인 요소 노드 추가
outline.AppendChildLast(outlineElem);

// 아웃라인 노드 추가
page.AppendChildLast(outline);

// 페이지 노드 추가
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### 또한보십시오

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


