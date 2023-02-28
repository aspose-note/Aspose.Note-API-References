---
title: PrintOptions.DocumentName
second_title: .NET API 참조용 Aspose.Note
description: PrintOptions 재산. 문서를 인쇄하는 동안 표시할 문서 이름예 인쇄 상태 대화 상자 또는 프린터 대기열을 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

문서를 인쇄하는 동안 표시할 문서 이름(예: 인쇄 상태 대화 상자 또는 프린터 대기열)을 가져오거나 설정합니다.

```csharp
public string DocumentName { get; set; }
```

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

* class [PrintOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../printoptions/)
* 집회 [Aspose.Note](../../../)


