---
title: Document.Print
second_title: Aspose.Note for .NET API 参考
description: Document 方法. 使用默认打印机打印文档
type: docs
weight: 130
url: /zh/net/aspose.note/document/print/
---
## Print() {#print}

使用默认打印机打印文档。

```csharp
public void Print()
```

### 例子

显示如何使用带有默认选项的标准 Windows 对话框将文档发送到打印机。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

使用默认打印机打印文档。

```csharp
public void Print(PrintOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| options | PrintOptions | 用于打印文档的选项。可以为 null. |

### 也可以看看

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


