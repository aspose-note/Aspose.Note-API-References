---
title: Class AlwaysSplitObjectsAlgorithm
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm 수업. 원본 페이지에 맞지 않는 경우 개체를 여러 부분으로 나눕니다.
type: docs
weight: 550
url: /ko/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

원본 페이지에 맞지 않는 경우 개체를 여러 부분으로 나눕니다.

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | 기본 생성자입니다. |

### 예

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


