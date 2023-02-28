---
title: RichText.Tags
second_title: .NET API 참조용 Aspose.Note
description: RichText 재산. 단락의 모든 태그 목록을 가져옵니다.
type: docs
weight: 90
url: /ko/net/aspose.note/richtext/tags/
---
## RichText.Tags property

단락의 모든 태그 목록을 가져옵니다.

```csharp
public List<ITag> Tags { get; }
```

### 예

Outlook의 작업 세부 정보에 액세스하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tasks();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// 모든 RichText 노드 가져오기
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 각 노드를 통해 반복
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // 속성 검색
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### 또한보십시오

* interface [ITag](../../itag/)
* class [RichText](../)
* 네임스페이스 [Aspose.Note](../../richtext/)
* 집회 [Aspose.Note](../../../)


