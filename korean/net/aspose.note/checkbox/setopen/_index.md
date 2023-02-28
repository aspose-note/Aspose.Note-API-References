---
title: CheckBox.SetOpen
second_title: .NET API 참조용 Aspose.Note
description: CheckBox 방법. 태그를 열린 상태로 설정합니다.
type: docs
weight: 80
url: /ko/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

태그를 열린 상태로 설정합니다.

```csharp
public virtual void SetOpen()
```

### 예

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

### 또한보십시오

* class [CheckBox](../)
* 네임스페이스 [Aspose.Note](../../checkbox/)
* 집회 [Aspose.Note](../../../)


