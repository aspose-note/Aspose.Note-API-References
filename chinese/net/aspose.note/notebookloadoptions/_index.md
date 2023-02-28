---
title: Class NotebookLoadOptions
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.NotebookLoadOptions 班级. 用于加载笔记本的选项
type: docs
weight: 420
url: /zh/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

用于加载笔记本的选项。

```csharp
public class NotebookLoadOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | 获取或设置一个值，指示子文档 是否应在以后显式加载。 |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | 获取或设置一个值，该值指示在加载父文档时是否应加载子文档 。 |

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

* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


