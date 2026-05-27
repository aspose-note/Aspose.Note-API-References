---
title: "类 NotebookSaveOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.NotebookSaveOptions 类。一个抽象基类，表示特定格式的笔记本保存选项"
type: docs
weight: 870
url: /zh/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

一个抽象基类，表示特定格式的笔记本保存选项。

```csharp
public abstract class NotebookSaveOptions
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 获取或设置一个值，指示是否应显式保存子文档。 |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | 获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。 |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | 获取笔记本保存的格式。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | 获取所有笔记本子文档的保存选项。 |

## 示例

展示如何以 PDF 格式保存扁平化的笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// 保存笔记本
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

展示如何将扁平化的笔记本保存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

### 另请参阅

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


