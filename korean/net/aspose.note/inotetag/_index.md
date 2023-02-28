---
title: Interface INoteTag
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.INoteTag 상호 작용. 메모 태그용 인터페이스예 Outlook 작업과 연결되지 않은 태그.
type: docs
weight: 180
url: /ko/net/aspose.note/inotetag/
---
## INoteTag interface

메모 태그용 인터페이스(예: Outlook 작업과 연결되지 않은 태그).

```csharp
public interface INoteTag : ITag
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | 글꼴 색상을 가져오거나 설정합니다. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | 하이라이트 색상을 가져오거나 설정합니다. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | 레이블 텍스트를 가져오거나 설정합니다. |

### 예

태그 세부 정보에 액세스하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "TagFile.one");

// 모든 RichText 노드 가져오기
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 각 노드를 통해 반복
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 속성 검색
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### 또한보십시오

* interface [ITag](../itag/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


