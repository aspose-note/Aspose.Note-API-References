---
title: ITag.CompletedTime
second_title: Aspose.Note for .NET API リファレンス
description: ITag 財産. 完了時間を取得または設定します
type: docs
weight: 10
url: /ja/net/aspose.note/itag/completedtime/
---
## ITag.CompletedTime property

完了時間を取得または設定します。

```csharp
public DateTime? CompletedTime { get; }
```

### プロパティ値

Nullable.

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

タグの詳細にアクセスする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "TagFile.one");

// すべての RichText ノードを取得します
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 各ノードを繰り返します
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // プロパティを取得する
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

### 関連項目

* interface [ITag](../)
* 名前空間 [Aspose.Note](../../itag/)
* 組み立て [Aspose.Note](../../../)


