---
title: "NoteTask.DueDate"
second_title: "Aspose.Note for .NET API 参考"
description: "NoteTask 属性。获取或设置截止日期"
type: docs
weight: 70
url: /zh/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

获取或设置截止日期。

```csharp
public DateTime DueDate { get; set; }
```

### Property Value

DateTime。

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

展示如何访问 Outlook 任务的详细信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有 RichText 节点
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 遍历每个节点
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

### 另请参阅

* class [NoteTask](../)
* namespace [Aspose.Note](../../notetask/)
* assembly [Aspose.Note](../../../)


