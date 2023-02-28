---
title: Class OneSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.OneSaveOptions 수업. 문서를 OneNote 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.
type: docs
weight: 810
url: /ko/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

문서를 OneNote 형식으로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | 문서 내용을 암호화하기 위한 암호를 가져오거나 설정합니다. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 를 저장하는 동안 사용할 글꼴 설정을 가져오거나 설정합니다. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 저장할 페이지 수를 가져오거나 설정합니다. 기본적으로MaxValue 문서의 모든 페이지가 렌더링됨을 의미합니다. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0. 입니다. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | 문서가 저장되는 형식을 가져옵니다. |

### 예

암호화로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

OneSaveOptions를 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### 또한보십시오

* class [SaveOptions](../saveoptions/)
* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


