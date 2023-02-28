---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note for .NET API 参考
description: LoadOptions 财产. 获取或设置加密文档内容的密码如果文档没有密码保护值将被忽略
type: docs
weight: 20
url: /zh/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

获取或设置加密文档内容的密码。如果文档没有密码保护，值将被忽略。

```csharp
public string DocumentPassword { get; set; }
```

### 例子

显示如何加密文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

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

* class [LoadOptions](../)
* 命名空间 [Aspose.Note](../../loadoptions/)
* 部件 [Aspose.Note](../../../)


