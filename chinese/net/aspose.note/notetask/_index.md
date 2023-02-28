---
title: Class NoteTask
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.NoteTask 班级. 代表一个笔记任务
type: docs
weight: 400
url: /zh/net/aspose.note/notetask/
---
## NoteTask class

代表一个笔记任务。

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | 获取CheckBox是否处于选中状态的值。 |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | 获取或设置完成时间。 |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | 获取或设置创建时间。 |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | 获取或设置截止日期。 |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | 获取或设置图标。 |
| [Label](../../aspose.note/checkbox/label/) { get; } | 获取标签文本。 |
| [Status](../../aspose.note/checkbox/status/) { get; } | 获取或设置状态。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | 创建一个带有 NoFollowUpDateFlag 图标和指定截止日期的新笔记任务。 |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | 创建一个带有 FollowUpNextWeekFlag 图标的新笔记任务。 |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | 创建一个带有 FollowUpThisWeekFlag 图标的新笔记任务。 |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | 创建一个带有 FollowUpTodayFlag 图标的新笔记任务。 |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | 创建一个带有 FollowUpTomorrowFlag 图标的新笔记任务。 |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | 创建一个带有 NoFollowUpDateFlag 图标的新笔记任务。 |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | 判断指定对象是否等于当前对象。 |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | 判断指定对象是否等于当前对象。 |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | 用作类型的哈希函数。 |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | 使用当前时间作为完成时间将标签设置为完成状态。 |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | 将标签设置为完成状态。 |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | 将标签设置为打开状态。 |

### 例子

显示如何生成包含与“项目 A”相关的所有页面的 pdf。

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

显示如何访问 outlook 任务的详细信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有 RichText 节点
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

//遍历每个节点
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // 检索属性
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### 也可以看看

* class [CheckBox](../checkbox/)
* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


