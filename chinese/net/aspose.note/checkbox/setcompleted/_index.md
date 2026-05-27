---
title: "CheckBox.SetCompleted"
second_title: "Aspose.Note for .NET API 参考"
description: "CheckBox 方法。将标签设置为已完成状态"
type: docs
weight: 70
url: /zh/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

将标签设置为已完成状态。

```csharp
public void SetCompleted(DateTime completedTime)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| completedTime | DateTime | 完成时间。 |

### 另请参阅

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

将标签设置为已完成状态，并使用当前时间作为完成时间。

```csharp
public void SetCompleted()
```

## 示例

展示如何将与 'Project C' 相关的所有复选框项目标记为已完成。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

### 另请参阅

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)


