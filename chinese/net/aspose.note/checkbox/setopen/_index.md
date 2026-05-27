---
title: "CheckBox.SetOpen"
second_title: "Aspose.Note for .NET API 参考"
description: "CheckBox 方法。将标签设置为打开状态"
type: docs
weight: 80
url: /zh/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

将标签设置为打开状态。

```csharp
public virtual void SetOpen()
```

## 示例

展示如何将与 'Project C' 相关的所有复选框项目标记为打开。

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

### 另请参阅

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)


