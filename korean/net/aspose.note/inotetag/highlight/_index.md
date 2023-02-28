---
title: INoteTag.Highlight
second_title: .NET API 참조용 Aspose.Note
description: INoteTag 재산. 하이라이트 색상을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

하이라이트 색상을 가져오거나 설정합니다.

```csharp
public Color Highlight { get; set; }
```

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

* interface [INoteTag](../)
* 네임스페이스 [Aspose.Note](../../inotetag/)
* 집회 [Aspose.Note](../../../)


