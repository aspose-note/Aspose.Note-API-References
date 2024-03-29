---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions 班级. 一个抽象基类表示特定格式的笔记本保存选项 并为所有文档子节点提供通用保存选项
type: docs
weight: 800
url: /zh/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

一个抽象基类，表示特定格式的笔记本保存选项 ，并为所有文档子节点提供通用保存选项。

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| 范围 | 描述 |
| --- | --- |
| TDocumentSaveOptions | 所有notebook子文档的保存选项。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 获取或设置一个值，该值指示是否应明确保存子文档 。 |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | 获取或设置所有笔记本子文档的保存选项。 |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 获取或设置一个值，该值指示笔记本子层次结构是否以扁平化方式保存。 |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | 获取保存笔记本的格式。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | 获取所有笔记本子文档的保存选项。 |

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

### 也可以看看

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving/)
* 部件 [Aspose.Note](../../)


