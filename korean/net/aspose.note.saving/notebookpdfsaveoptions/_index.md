---
title: Class NotebookPdfSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.NotebookPdfSaveOptions 수업. 노트북 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
type: docs
weight: 780
url: /ko/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

노트북 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 하위 문서 를 명시적으로 저장해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 노트북 하위 계층이 평면화되어 저장되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


