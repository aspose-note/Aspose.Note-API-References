---
title: NotebookLoadOptions.DeferredLoading
second_title: .NET API 참조용 Aspose.Note
description: NotebookLoadOptions 재산. 하위 문서 를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

하위 문서 를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool DeferredLoading { get; set; }
```

### 비고

기본값은`거짓` , 하위 문서가 암시적으로 로드됩니다. 값`진실` 사용자가 전화해야 함을 나타냅니다.[`LoadChildDocument`](../../notebook/loadchilddocument/) 또는 노트북 자체가 로드된 후 각 노트북의 하위 노드에 대해. 값이 다음과 같은 경우`진실` ,[`InstantLoading`](../instantloading/) 옵션은 무시됩니다. 노트북이 스트림에서 로드되는 경우 값은 항상`진실` 사용자가 명시적으로 설정했음에도 불구하고`거짓` .

### 예

노트북을 암호화하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### 또한보십시오

* class [NotebookLoadOptions](../)
* 네임스페이스 [Aspose.Note](../../notebookloadoptions/)
* 집회 [Aspose.Note](../../../)


