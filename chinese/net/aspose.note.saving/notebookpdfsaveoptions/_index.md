---
title: "类 NotebookPdfSaveOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.NotebookPdfSaveOptions 类。允许在将笔记本页面渲染为 PDF 时指定其他选项"
type: docs
weight: 860
url: /zh/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

允许在将笔记本页面渲染为 PDF 时指定其他选项。

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 获取或设置一个值，指示是否应显式保存子文档。 |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。 |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

### 另请参阅

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


