---
title: "NotebookLoadOptions.DeferredLoading"
second_title: "Aspose.Note for .NET API 参考"
description: "NotebookLoadOptions 属性。获取或设置一个值，指示是否应稍后显式加载子文档。"
type: docs
weight: 20
url: /zh/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

获取或设置一个值，指示是否应稍后显式加载子文档。

```csharp
public bool DeferredLoading { get; set; }
```

## 备注

默认值为 `false`，因此子文档将隐式加载。值为 `true` 表示用户应在笔记本本身加载后，调用 [`LoadChildDocument`](../../notebook/loadchilddocument/) 或 为每个笔记本的子节点进行加载。如果值为 `true`，[`InstantLoading`](../instantloading/) 选项将被忽略。如果笔记本是从流中加载的，无论用户是否显式设置为 `false`，该值始终为 `true`。

## 示例

展示如何打开加密的笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### 另请参阅

* class [NotebookLoadOptions](../)
* namespace [Aspose.Note](../../notebookloadoptions/)
* assembly [Aspose.Note](../../../)


