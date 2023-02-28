---
title: CheckBox.SetCompleted
second_title: .NET API 참조용 Aspose.Note
description: CheckBox 방법. 태그를 완료 상태로 설정합니다.
type: docs
weight: 70
url: /ko/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

태그를 완료 상태로 설정합니다.

```csharp
public void SetCompleted(DateTime completedTime)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| completedTime | DateTime | 완료된 시간. |

### 또한보십시오

* class [CheckBox](../)
* 네임스페이스 [Aspose.Note](../../checkbox/)
* 집회 [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

현재 시간을 완료 시간으로 사용하여 태그를 완료 상태로 설정합니다.

```csharp
public void SetCompleted()
```

### 예

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

### 또한보십시오

* class [CheckBox](../)
* 네임스페이스 [Aspose.Note](../../checkbox/)
* 집회 [Aspose.Note](../../../)


