---
title: RichText.Tags
second_title: Aspose.Note for .NET API 参考
description: RichText 财产. 获取段落的所有标签列表
type: docs
weight: 90
url: /zh/net/aspose.note/richtext/tags/
---
## RichText.Tags property

获取段落的所有标签列表。

```csharp
public List<ITag> Tags { get; }
```

### 例子

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

* interface [ITag](../../itag/)
* class [RichText](../)
* 命名空间 [Aspose.Note](../../richtext/)
* 部件 [Aspose.Note](../../../)


