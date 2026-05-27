---
title: "Notebook.DisplayName"
second_title: "Aspose.Note for .NET API 参考"
description: "Notebook 属性。获取或设置显示名称"
type: docs
weight: 40
url: /zh/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

获取或设置显示名称。

```csharp
public string DisplayName { get; set; }
```

## 示例

展示如何从笔记本中删除章节。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "test.onetoc2");

// 遍历其子节点以搜索所需的子项
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

### 另请参阅

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


