---
title: Class NotebookSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.NotebookSaveOptions 수업. 특정 형식에 대한 노트북 저장 옵션을 나타내는 추상 기본 클래스입니다.
type: docs
weight: 790
url: /ko/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

특정 형식에 대한 노트북 저장 옵션을 나타내는 추상 기본 클래스입니다.

```csharp
public abstract class NotebookSaveOptions
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 하위 문서 를 명시적으로 저장해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 노트북 하위 계층이 평면화되어 저장되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | 노트북이 저장되는 형식을 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | 모든 노트북의 하위 문서에 대한 저장 옵션을 가져옵니다. |

### 예

결합된 노트북을 pdf 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 노트북 저장
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

병합된 노트북을 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 노트북 저장
notebook.Save(dataDir, notebookSaveOptions);
```

### 또한보십시오

* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


