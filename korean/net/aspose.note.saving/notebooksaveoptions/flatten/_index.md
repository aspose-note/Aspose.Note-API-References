---
title: NotebookSaveOptions.Flatten
second_title: .NET API 참조용 Aspose.Note
description: NotebookSaveOptions 재산. 노트북 하위 계층이 평면화되어 저장되는지 여부를 나타내는 값을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

노트북 하위 계층이 평면화되어 저장되는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool Flatten { get; set; }
```

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

* class [NotebookSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../notebooksaveoptions/)
* 집회 [Aspose.Note](../../../)


