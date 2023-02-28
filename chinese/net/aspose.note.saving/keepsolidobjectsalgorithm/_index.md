---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm 班级. 将整个对象移至下一页以防原始页面放不下
type: docs
weight: 740
url: /zh/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

将整个对象移至下一页，以防原始页面放不下。

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | 初始化一个新的实例`KeepSolidObjectsAlgorithm`使用克隆部分的默认高度限制的类. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | 初始化一个新的实例`KeepSolidObjectsAlgorithm`使用克隆部分的特定高度限制的类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | 获取克隆部分的高度限制。 |

## 字段

| 姓名 | 描述 |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | 克隆部分的默认最大大小。 |

### 例子

显示如何使用指定选项将笔记本保存为 pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载一个 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

显示如何使用具有指定选项的标准 Windows 对话框将文档发送到打印机。

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

当 OneNote 长页面以 pdf 格式保存时，它们会被拆分成多个页面。该示例显示如何配置位于分页符处的对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### 也可以看看

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving/)
* 部件 [Aspose.Note](../../)


