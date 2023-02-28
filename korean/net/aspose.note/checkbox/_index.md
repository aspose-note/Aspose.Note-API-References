---
title: Class CheckBox
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.CheckBox 수업. 완료와 미완료 사이에서 상태를 전환할 수 있는 태그의 기본 클래스입니다.
type: docs
weight: 20
url: /ko/net/aspose.note/checkbox/
---
## CheckBox class

완료와 미완료 사이에서 상태를 전환할 수 있는 태그의 기본 클래스입니다.

```csharp
public abstract class CheckBox : ITag
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | CheckBox가 체크 상태인지 여부를 나타내는 값을 가져옵니다. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | 완료된 시간을 가져오거나 설정합니다. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | 생성 시간을 가져오거나 설정합니다. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | 아이콘을 가져오거나 설정합니다. |
| [Label](../../aspose.note/checkbox/label/) { get; } | 레이블 텍스트를 가져옵니다. |
| [Status](../../aspose.note/checkbox/status/) { get; } | 상태를 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | 현재 시간을 완료 시간으로 사용하여 태그를 완료 상태로 설정합니다. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | 태그를 완료 상태로 설정합니다. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | 태그를 열린 상태로 설정합니다. |

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

'Project C'와 관련된 모든 체크박스 항목을 완료하게 만드는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

'Project C'와 관련된 모든 체크박스 항목을 여는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

불완전한 확인란으로 표시되고 지난주에 생성된 항목이 포함된 페이지가 포함된 PDF를 생성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

이번 주에 완료해야 하는 Outlook 미완료 작업이 포함된 페이지가 포함된 PDF를 생성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Tags();

// 문서를 Aspose.Note에 로드합니다.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

### 또한보십시오

* interface [ITag](../itag/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


