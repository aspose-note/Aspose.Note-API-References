---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: NotebookSaveOptions 재산. 모든 노트북의 하위 문서에 대한 저장 옵션을 가져오거나 설정합니다.
type: docs
weight: 10
url: /ko/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

모든 노트북의 하위 문서에 대한 저장 옵션을 가져오거나 설정합니다.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### 예

지정된 옵션을 사용하여 노트북을 pdf 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// 노트북 저장
notebook.Save(dataDir, notebookSaveOptions);
```

### 또한보십시오

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* 네임스페이스 [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* 집회 [Aspose.Note](../../../)


