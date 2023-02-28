---
title: Notebook.RemoveChild
second_title: Aspose.Note for .NET API 参考
description: Notebook 方法. 删除子节点
type: docs
weight: 140
url: /zh/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

删除子节点。

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| oldChild | INotebookChildNode | 要删除的节点。 |

### 返回值

删除的节点。

### 例子

显示如何从笔记本访问所有部分。

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
```

演示如何从笔记本中删除部分。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载一个 OneNote 笔记本
var notebook = new Notebook(dataDir + "test.onetoc2");

//遍历其子节点以搜索所需的子项
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // 从笔记本中删除子项
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// 保存笔记本
notebook.Save(dataDir);
```

演示如何保存笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### 也可以看看

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* 命名空间 [Aspose.Note](../../notebook/)
* 部件 [Aspose.Note](../../../)


