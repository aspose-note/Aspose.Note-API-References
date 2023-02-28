---
title: CheckBox.SetOpen
second_title: Aspose.Note for .NET API 参考
description: CheckBox 方法. 将标签设置为打开状态
type: docs
weight: 80
url: /zh/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

将标签设置为打开状态。

```csharp
public virtual void SetOpen()
```

### 例子

显示如何打开与“项目 C”相关的所有复选框项目。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

### 也可以看看

* class [CheckBox](../)
* 命名空间 [Aspose.Note](../../checkbox/)
* 部件 [Aspose.Note](../../../)


