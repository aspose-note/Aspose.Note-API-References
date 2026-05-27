---
title: "类 KeepSolidObjectsAlgorithm"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.KeepSolidObjectsAlgorithm 类。若完整对象不适合原始页面，则将其移至下一页"
type: docs
weight: 820
url: /zh/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

在对象无法适应原始页面时，将完整对象移至下一页。

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | 使用克隆部分的默认高度限制初始化 `KeepSolidObjectsAlgorithm` 类的新实例。 |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | 使用克隆部分的特定高度限制初始化 `KeepSolidObjectsAlgorithm` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | 获取克隆部件的高度限制。 |

## 字段

| 名称 | 描述 |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | 克隆部件的默认最大尺寸。 |

## 示例

展示如何使用指定选项将笔记本保存为 PDF 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

展示如何使用标准 Windows 对话框并指定选项将文档发送到打印机。

```csharp
// 文档目录的路径。
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

当长的 OneNote 页面以 PDF 格式保存时，它们会被拆分到多个页面。示例展示如何配置位于页面换行处对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### 另请参阅

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


