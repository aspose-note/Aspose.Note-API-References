---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note for .NET API 参考
description: NotebookLoadOptions 财产. 获取或设置一个值指示子文档 是否应在以后显式加载
type: docs
weight: 20
url: /zh/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

获取或设置一个值，指示子文档 是否应在以后显式加载。

```csharp
public bool DeferredLoading { get; set; }
```

### 评论

默认值为`错误的` , 因此子文档将被隐式加载。 值`真的`表示用户应该调用[`LoadChildDocument`](../../notebook/loadchilddocument/)或者 用于笔记本本身加载后的每个笔记本的子节点。 如果值为`真的`,[`InstantLoading`](../instantloading/)选项将被忽略。 如果笔记本从流中加载，则该值始终为`真的`尽管被用户明确设置为`错误的`.

### 例子

展示如何加密笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### 也可以看看

* class [NotebookLoadOptions](../)
* 命名空间 [Aspose.Note](../../notebookloadoptions/)
* 部件 [Aspose.Note](../../../)


