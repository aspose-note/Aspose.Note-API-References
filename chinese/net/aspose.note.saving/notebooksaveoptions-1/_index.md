---
title: "类 NotebookSaveOptionsTDocumentSaveOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions 类。一个抽象基类，表示特定格式的笔记本保存选项，并为所有文档子节点提供通用的保存选项"
type: docs
weight: 880
url: /zh/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

一个抽象基类，表示特定格式的笔记本保存选项，并为所有文档子节点提供通用的保存选项。

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| 参数 | 描述 |
| --- | --- |
| TDocumentSaveOptions | 所有笔记本子文档的保存选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 获取或设置一个值，指示是否应显式保存子文档。 |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | 获取或设置所有笔记本子文档的保存选项。 |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。 |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | 获取笔记本保存的格式。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | 获取所有笔记本子文档的保存选项。 |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


