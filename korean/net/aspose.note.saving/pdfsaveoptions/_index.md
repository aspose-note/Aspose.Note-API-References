---
title: Class PdfSaveOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.PdfSaveOptions 수업. 문서 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
type: docs
weight: 850
url: /ko/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

문서 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 를 저장하는 동안 사용할 글꼴 설정을 가져오거나 설정합니다. |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | PDF 파일의 이미지에 적용되는 압축 유형을 가져오거나 설정합니다. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | PDF 문서 내 JPEG 이미지의 품질을 결정하는 값을 가져오거나 설정합니다. 값은 0에서 100까지 다양할 수 있습니다. 여기서 0은 품질이 가장 낮지만 최대 압축률을 의미하고 100은 최상의 품질이지만 최소 압축률을 의미합니다. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 저장할 페이지 수를 가져오거나 설정합니다. 기본적으로MaxValue 문서의 모든 페이지가 렌더링됨을 의미합니다. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0. 입니다. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | 문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. 기본적으로 CurrentUICulture에 따라 다름, *미국 문화에는 문자 설정이 있고 다른 문화에는 A4 설정이 있습니다. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | 문서가 저장되는 형식을 가져옵니다. |

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

긴 OneNote 페이지가 pdf 형식으로 저장되면 여러 페이지로 분할됩니다. 이 샘플은 페이지 나누기에 있는 개체의 분할 논리를 구성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

PDF 형식으로 문서를 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions 객체 초기화
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 저장할 첫 번째 페이지의 페이지 인덱스 설정
                              PageIndex = 0,

                              // 페이지 수 설정
                              PageCount = 1,
                          };

// 문서를 PDF로 저장
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

특정 설정을 사용하여 문서를 PDF 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions 객체 초기화
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Jpeg 압축 사용
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 압축 품질
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

긴 OneNote 페이지가 pdf 형식으로 저장되면 여러 페이지로 분할됩니다. 이 예는 페이지 나누기에 있는 개체의 분할 논리를 구성하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 문서를 Aspose.Note에 로드합니다.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 또는
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### 또한보십시오

* class [SaveOptions](../saveoptions/)
* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


