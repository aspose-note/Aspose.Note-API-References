---
title: Notebook.DisplayName
second_title: .NET API 참조용 Aspose.Note
description: Notebook 재산. 표시 이름을 가져오거나 설정합니다.
type: docs
weight: 40
url: /ko/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

표시 이름을 가져오거나 설정합니다.

```csharp
public string DisplayName { get; set; }
```

### 예

전자 필기장에서 섹션을 제거하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "test.onetoc2");

// 원하는 자식 항목을 검색하기 위해 자식 노드를 통과합니다.
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // 노트북에서 하위 항목 제거
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// 노트북 저장
notebook.Save(dataDir);
```

### 또한보십시오

* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)


