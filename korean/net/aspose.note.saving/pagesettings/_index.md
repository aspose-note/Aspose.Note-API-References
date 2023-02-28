---
title: Class PageSettings
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.PageSettings 수업. 페이지의 레이아웃 설정을 나타냅니다.
type: docs
weight: 820
url: /ko/net/aspose.note.saving/pagesettings/
---
## PageSettings class

페이지의 레이아웃 설정을 나타냅니다.

```csharp
public class PageSettings
```

## 속성

| 이름 | 설명 |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | A4 형식 페이지에 대한 설정을 가져옵니다. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | 높이 제한이 없는 A4 형식 페이지에 대한 설정을 가져옵니다. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Letter 형식 페이지에 대한 설정을 가져옵니다. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | 높이 제한이 없는 Letter 형식 페이지에 대한 설정을 가져옵니다. |

### 예

Letter 페이지 레이아웃을 사용하여 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// 문서를 저장합니다.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

높이 제한 없이 A4 페이지 레이아웃으로 PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// 문서를 저장합니다.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### 또한보십시오

* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


