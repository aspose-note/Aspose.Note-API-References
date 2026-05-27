---
title: "类 CheckBox"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.CheckBox 类。用于在完成和未完成之间切换状态的标签的基类"
type: docs
weight: 20
url: /zh/net/aspose.note/checkbox/
---
## CheckBox class

用于在完成和未完成之间切换状态的标签的基类。

```csharp
public abstract class CheckBox : ITag
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | 获取一个值，指示复选框是否处于选中状态。 |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | 获取或设置完成时间。 |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | 获取或设置创建时间。 |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | 获取或设置图标。 |
| [Label](../../aspose.note/checkbox/label/) { get; } | 获取标签文本。 |
| [Status](../../aspose.note/checkbox/status/) { get; } | 获取或设置状态。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | 将标签设置为已完成状态，并使用当前时间作为完成时间。 |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | 将标签设置为已完成状态。 |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | 将标签设置为打开状态。 |

## 示例

展示如何生成包含所有与‘Project A’相关页面的 PDF。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

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

展示如何生成包含上周创建且标记为未完成复选框的页面的 PDF。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

展示如何生成包含本周需完成的 Outlook 未完成任务页面的 PDF。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

### 另请参阅

* interface [ITag](../itag/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


