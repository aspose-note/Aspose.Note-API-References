---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions 수업. 특정 format 에 대한 노트북 저장 옵션을 나타내고 모든 문서 하위 노드에 대한 공통 저장 옵션을 제공하는 추상 기본 클래스입니다.
type: docs
weight: 800
url: /ko/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

특정 format 에 대한 노트북 저장 옵션을 나타내고 모든 문서 하위 노드에 대한 공통 저장 옵션을 제공하는 추상 기본 클래스입니다.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| 모수 | 설명 |
| --- | --- |
| TDocumentSaveOptions | 모든 노트북의 하위 문서에 대한 저장 옵션입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 하위 문서 를 명시적으로 저장해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | 모든 노트북의 하위 문서에 대한 저장 옵션을 가져오거나 설정합니다. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 노트북 하위 계층이 평면화되어 저장되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | 노트북이 저장되는 형식을 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | 모든 노트북의 하위 문서에 대한 저장 옵션을 가져옵니다. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


