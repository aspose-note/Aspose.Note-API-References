---
title: INoteTag.Highlight
second_title: Aspose.Note for .NET API 参考
description: INoteTag 财产. 获取或设置高亮颜色
type: docs
weight: 20
url: /zh/net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

获取或设置高亮颜色。

```csharp
public Color Highlight { get; set; }
```

### 例子

显示如何访问标签的详细信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "TagFile.one");

// 获取所有 RichText 节点
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

//遍历每个节点
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 检索属性
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### 也可以看看

* interface [INoteTag](../)
* 命名空间 [Aspose.Note](../../inotetag/)
* 部件 [Aspose.Note](../../../)


