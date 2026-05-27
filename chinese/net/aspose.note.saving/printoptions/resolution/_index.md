---
title: "PrintOptions.Resolution"
second_title: "Aspose.Note for .NET API 参考"
description: "PrintOptions 属性。获取或设置生成图像的分辨率（每英寸点数）"
type: docs
weight: 50
url: /zh/net/aspose.note.saving/printoptions/resolution/
---
## PrintOptions.Resolution property

获取或设置生成图像的分辨率（每英寸点数）。

```csharp
public float Resolution { get; set; }
```

## 备注

默认值为 96。

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

* class [PrintOptions](../)
* namespace [Aspose.Note.Saving](../../printoptions/)
* assembly [Aspose.Note](../../../)


