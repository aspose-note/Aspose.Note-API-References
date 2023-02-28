---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm 수업. 개체의 상단 부분을 페이지 하단에 추가하고 원본 페이지에 맞지 않는 경우 전체 개체를 다음 페이지에 복제합니다.
type: docs
weight: 730
url: /ko/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

개체의 상단 부분을 페이지 하단에 추가하고 원본 페이지에 맞지 않는 경우 전체 개체를 다음 페이지에 복제합니다.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | 의 새 인스턴스를 초기화합니다.`KeepPartAndCloneSolidObjectToNextPageAlgorithm` 클래스, 복제된 부품의 기본 높이 제한 사용. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | 의 새 인스턴스를 초기화합니다.`KeepPartAndCloneSolidObjectToNextPageAlgorithm` 클래스, 복제된 부품의 특정 높이 제한 사용. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | 복제된 부품의 높이 제한을 가져옵니다. |

## 필드

| 이름 | 설명 |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | 복제된 부품의 기본 최대 크기입니다. |

### 예

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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


