---
title: PrintOptions.PageSplittingAlgorithm
second_title: .NET API 참조용 Aspose.Note
description: PrintOptions 재산. 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다.
type: docs
weight: 30
url: /ko/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### 자산 가치

`PageSplittingAlgorithm` .

### 예

지정된 옵션과 함께 표준 Windows 대화 상자를 사용하여 문서를 프린터로 보내는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### 또한보십시오

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../printoptions/)
* 집회 [Aspose.Note](../../../)


