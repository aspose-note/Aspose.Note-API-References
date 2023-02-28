---
title: PdfSaveOptions.PageSettings
second_title: .NET API 참조용 Aspose.Note
description: PdfSaveOptions 재산. 문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. 기본적으로 CurrentUICulture에 따라 다름 미국 문화에는 문자 설정이 있고 다른 문화에는 A4 설정이 있습니다.
type: docs
weight: 40
url: /ko/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. 기본적으로 CurrentUICulture에 따라 다름, *미국 문화에는 문자 설정이 있고 다른 문화에는 A4 설정이 있습니다.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 집회 [Aspose.Note](../../../)


