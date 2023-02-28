---
title: Class NoteTask
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.NoteTask クラス. メモタスクを表します.
type: docs
weight: 400
url: /ja/net/aspose.note/notetask/
---
## NoteTask class

メモタスクを表します.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | CheckBox がチェックされた状態かどうかを示す値を取得します。 |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | 完了時間を取得または設定します。 |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | 作成時刻を取得または設定します。 |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | 期日を取得または設定します。 |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | アイコンを取得または設定します。 |
| [Label](../../aspose.note/checkbox/label/) { get; } | ラベル テキストを取得します。 |
| [Status](../../aspose.note/checkbox/status/) { get; } | ステータスを取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | NoFollowUpDateFlag アイコンと期日を指定して、新しいメモ タスクを作成します。 |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | FollowUpNextWeekFlag アイコンで新しいノート タスクを作成します。 |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | FollowUpThisWeekFlag アイコンで新しいノート タスクを作成します。 |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | FollowUpTodayFlag アイコンで新しいノート タスクを作成します。 |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | FollowUpTomorrowFlag アイコンで新しいノート タスクを作成します。 |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | NoFollowUpDateFlag アイコンで新しいノート タスクを作成します。 |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | タイプのハッシュ関数として機能します。 |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | 現在時刻を完了時刻としてタグを完了状態に設定します。 |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | タグを完了状態に設定します。 |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | タグをオープン状態に設定します。 |

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

* class [CheckBox](../checkbox/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


