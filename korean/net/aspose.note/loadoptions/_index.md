---
title: Class LoadOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.LoadOptions 수업. 문서를 로드하는 데 사용되는 옵션입니다.
type: docs
weight: 320
url: /ko/net/aspose.note/loadoptions/
---
## LoadOptions class

문서를 로드하는 데 사용되는 옵션입니다.

```csharp
public class LoadOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [LoadOptions](loadoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | 암호화된 문서 콘텐츠의 암호를 가져오거나 설정합니다. 문서가 암호로 보호되지 않은 경우 값이 무시됩니다. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | 문서 로더가 기록을 무시해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. 이 옵션을 사용하여 메모리 및 CPU 사용량을 줄입니다. 기본값은 다음과 같습니다.`진실` . |

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

페이지 기록을 가져오는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote 문서 로드
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 첫 페이지 가져오기
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### 또한보십시오

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


