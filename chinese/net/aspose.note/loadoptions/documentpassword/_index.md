---
title: "LoadOptions.DocumentPassword"
second_title: "Aspose.Note for .NET API 参考"
description: "LoadOptions 属性。获取或设置加密文档内容的密码。如果文档未受密码保护，则该值将被忽略。"
type: docs
weight: 20
url: /zh/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

获取或设置加密文档内容的密码。如果文档未受密码保护，则此值将被忽略。

```csharp
public string DocumentPassword { get; set; }
```

## 示例

展示如何处理加密文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

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

* class [LoadOptions](../)
* namespace [Aspose.Note](../../loadoptions/)
* assembly [Aspose.Note](../../../)


