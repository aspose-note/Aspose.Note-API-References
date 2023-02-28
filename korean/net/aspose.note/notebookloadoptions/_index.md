---
title: Class NotebookLoadOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.NotebookLoadOptions 수업. 노트북을 로드하는 데 사용되는 옵션입니다.
type: docs
weight: 420
url: /ko/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

노트북을 로드하는 데 사용되는 옵션입니다.

```csharp
public class NotebookLoadOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | 하위 문서 를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | 상위 문서가 로드되는 동안 하위 문서 를 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |

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

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


