---
title: RichText.Tags
second_title: Aspose.Note for .NET API リファレンス
description: RichText 財産. 段落のすべてのタグのリストを取得します
type: docs
weight: 90
url: /ja/net/aspose.note/richtext/tags/
---
## RichText.Tags property

段落のすべてのタグのリストを取得します。

```csharp
public List<ITag> Tags { get; }
```

### 例

Outlook のタスクの詳細にアクセスする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tasks();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての RichText ノードを取得します
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 各ノードを繰り返します
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // プロパティを取得する
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### 関連項目

* interface [ITag](../../itag/)
* class [RichText](../)
* 名前空間 [Aspose.Note](../../richtext/)
* 組み立て [Aspose.Note](../../../)


