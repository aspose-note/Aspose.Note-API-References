---
title: "类 NotebookLoadOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.NotebookLoadOptions 类。用于加载笔记本的选项"
type: docs
weight: 490
url: /zh/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

用于加载笔记本的选项。

```csharp
public class NotebookLoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | 获取或设置一个值，指示是否应稍后显式加载子文档。 |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | 获取或设置一个值，指示是否在加载父文档时加载子文档。 |

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


