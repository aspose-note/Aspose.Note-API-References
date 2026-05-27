---
title: "类 PrintOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.PrintOptions 类。用于打印文档的选项"
type: docs
weight: 940
url: /zh/net/aspose.note.saving/printoptions/
---
## PrintOptions class

用于打印文档的选项。

```csharp
public class PrintOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrintOptions](printoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | 获取或设置在打印文档时显示的文档名称（例如，在打印状态对话框或打印队列中）。 |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | 获取或设置用于页面拆分的算法。 |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | 获取或设置打印机设置。 |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | 获取或设置生成图像的分辨率（每英寸点数）。 |

## 示例

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

### 另请参阅

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


