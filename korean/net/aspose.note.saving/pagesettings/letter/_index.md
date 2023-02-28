---
title: PageSettings.Letter
second_title: .NET API 참조용 Aspose.Note
description: PageSettings 재산. Letter 형식 페이지에 대한 설정을 가져옵니다.
type: docs
weight: 30
url: /ko/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Letter 형식 페이지에 대한 설정을 가져옵니다.

```csharp
public static PageSettings Letter { get; }
```

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

### 또한보십시오

* class [PageSettings](../)
* 네임스페이스 [Aspose.Note.Saving](../../pagesettings/)
* 집회 [Aspose.Note](../../../)


