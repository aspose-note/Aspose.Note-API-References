---
title: Class PrintOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Saving.PrintOptions 수업. 문서를 인쇄하는 데 사용되는 옵션입니다.
type: docs
weight: 860
url: /ko/net/aspose.note.saving/printoptions/
---
## PrintOptions class

문서를 인쇄하는 데 사용되는 옵션입니다.

```csharp
public class PrintOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PrintOptions](printoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | 문서를 인쇄하는 동안 표시할 문서 이름(예: 인쇄 상태 대화 상자 또는 프린터 대기열)을 가져오거나 설정합니다. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | 프린터 설정을 가져오거나 설정합니다. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | 생성된 이미지의 해상도를 인치당 도트 수로 가져오거나 설정합니다. |

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

* 네임스페이스 [Aspose.Note.Saving](../../aspose.note.saving/)
* 집회 [Aspose.Note](../../)


