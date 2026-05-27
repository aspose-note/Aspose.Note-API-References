---
title: "NotebookSaveOptions1.DocumentSaveOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "NotebookSaveOptions 属性。获取或设置所有笔记本子文档的保存选项"
type: docs
weight: 10
url: /zh/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

获取或设置所有笔记本子文档的保存选项。

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* assembly [Aspose.Note](../../../)


