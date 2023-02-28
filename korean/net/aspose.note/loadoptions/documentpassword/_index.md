---
title: LoadOptions.DocumentPassword
second_title: .NET API 참조용 Aspose.Note
description: LoadOptions 재산. 암호화된 문서 콘텐츠의 암호를 가져오거나 설정합니다. 문서가 암호로 보호되지 않은 경우 값이 무시됩니다.
type: docs
weight: 20
url: /ko/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

암호화된 문서 콘텐츠의 암호를 가져오거나 설정합니다. 문서가 암호로 보호되지 않은 경우 값이 무시됩니다.

```csharp
public string DocumentPassword { get; set; }
```

### 예

문서를 암호화하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

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

* class [LoadOptions](../)
* 네임스페이스 [Aspose.Note](../../loadoptions/)
* 집회 [Aspose.Note](../../../)


