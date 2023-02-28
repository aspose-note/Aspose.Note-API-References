---
title: Class NoteTask
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.NoteTask 수업. 메모 작업을 나타냅니다.
type: docs
weight: 400
url: /ko/net/aspose.note/notetask/
---
## NoteTask class

메모 작업을 나타냅니다.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | CheckBox가 체크 상태인지 여부를 나타내는 값을 가져옵니다. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | 완료된 시간을 가져오거나 설정합니다. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | 생성 시간을 가져오거나 설정합니다. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | 기한을 가져오거나 설정합니다. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | 아이콘을 가져오거나 설정합니다. |
| [Label](../../aspose.note/checkbox/label/) { get; } | 레이블 텍스트를 가져옵니다. |
| [Status](../../aspose.note/checkbox/status/) { get; } | 상태를 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | NoFollowUpDateFlag 아이콘 및 지정된 기한을 사용하여 새 메모 작업을 만듭니다. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | FollowUpNextWeekFlag 아이콘으로 새 메모 작업을 만듭니다. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | FollowUpThisWeekFlag 아이콘으로 새 메모 작업을 만듭니다. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | FollowUpTodayFlag 아이콘으로 새 메모 작업을 만듭니다. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | FollowUpTomorrowFlag 아이콘으로 새 메모 작업을 만듭니다. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | NoFollowUpDateFlag 아이콘으로 새 메모 작업을 만듭니다. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | 지정된 개체가 현재 개체와 같은지 여부를 결정합니다. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | 유형에 대한 해시 함수 역할을 합니다. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | 현재 시간을 완료 시간으로 사용하여 태그를 완료 상태로 설정합니다. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | 태그를 완료 상태로 설정합니다. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | 태그를 열린 상태로 설정합니다. |

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

* class [CheckBox](../checkbox/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


