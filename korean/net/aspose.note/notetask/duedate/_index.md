---
title: NoteTask.DueDate
second_title: .NET API 참조용 Aspose.Note
description: NoteTask 재산. 기한을 가져오거나 설정합니다.
type: docs
weight: 70
url: /ko/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

기한을 가져오거나 설정합니다.

```csharp
public DateTime DueDate { get; set; }
```

### 자산 가치

DateTime .

### 예

'프로젝트 A'와 관련된 모든 페이지가 포함된 PDF를 생성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

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

* class [NoteTask](../)
* 네임스페이스 [Aspose.Note](../../notetask/)
* 집회 [Aspose.Note](../../../)


