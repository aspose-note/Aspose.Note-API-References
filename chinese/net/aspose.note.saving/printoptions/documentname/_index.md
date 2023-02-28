---
title: PrintOptions.DocumentName
second_title: Aspose.Note for .NET API 参考
description: PrintOptions 财产. 获取或设置打印文档时要显示的文档名称例如在打印状态对话框或打印机队列中
type: docs
weight: 20
url: /zh/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

获取或设置打印文档时要显示的文档名称（例如，在打印状态对话框或打印机队列中）。

```csharp
public string DocumentName { get; set; }
```

### 例子

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

### 也可以看看

* class [PrintOptions](../)
* 命名空间 [Aspose.Note.Saving](../../printoptions/)
* 部件 [Aspose.Note](../../../)


