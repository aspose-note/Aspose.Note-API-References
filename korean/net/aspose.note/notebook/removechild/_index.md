---
title: Notebook.RemoveChild
second_title: .NET API 참조용 Aspose.Note
description: Notebook 방법. 자식 노드를 제거합니다.
type: docs
weight: 140
url: /ko/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

자식 노드를 제거합니다.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| oldChild | INotebookChildNode | 제거할 노드입니다. |

### 반환 값

제거된 노드입니다.

### 예

노트북에서 모든 섹션에 액세스하는 방법을 보여줍니다.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
```

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

노트북을 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### 또한보십시오

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)


