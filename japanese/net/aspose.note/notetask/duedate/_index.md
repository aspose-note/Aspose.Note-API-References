---
title: NoteTask.DueDate
second_title: Aspose.Note for .NET API リファレンス
description: NoteTask 財産. 期日を取得または設定します
type: docs
weight: 70
url: /ja/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

期日を取得または設定します。

```csharp
public DateTime DueDate { get; set; }
```

### プロパティ値

DateTime.

### 例

「プロジェクト A」に関連するすべてのページを含む PDF を生成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
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

* class [NoteTask](../)
* 名前空間 [Aspose.Note](../../notetask/)
* 組み立て [Aspose.Note](../../../)


