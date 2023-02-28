---
title: Document.Print
second_title: .NET API 참조용 Aspose.Note
description: Document 방법. 기본 프린터를 사용하여 문서를 인쇄합니다.
type: docs
weight: 130
url: /ko/net/aspose.note/document/print/
---
## Print() {#print}

기본 프린터를 사용하여 문서를 인쇄합니다.

```csharp
public void Print()
```

### 예

기본 옵션이 있는 표준 Windows 대화 상자를 사용하여 문서를 프린터로 보내는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

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

* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

기본 프린터를 사용하여 문서를 인쇄합니다.

```csharp
public void Print(PrintOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| options | PrintOptions | 문서를 인쇄하는 데 사용되는 옵션입니다. null일 수 있습니다. |

### 또한보십시오

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


