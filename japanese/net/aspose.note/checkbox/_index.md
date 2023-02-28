---
title: Class CheckBox
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.CheckBox クラス. 状態を完了と未完了の間で切り替えることができるタグの基本クラス
type: docs
weight: 20
url: /ja/net/aspose.note/checkbox/
---
## CheckBox class

状態を完了と未完了の間で切り替えることができるタグの基本クラス。

```csharp
public abstract class CheckBox : ITag
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | CheckBox がチェックされた状態かどうかを示す値を取得します。 |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | 完了時間を取得または設定します。 |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | 作成時刻を取得または設定します。 |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | アイコンを取得または設定します。 |
| [Label](../../aspose.note/checkbox/label/) { get; } | ラベル テキストを取得します。 |
| [Status](../../aspose.note/checkbox/status/) { get; } | ステータスを取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | 現在時刻を完了時刻としてタグを完了状態に設定します。 |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | タグを完了状態に設定します。 |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | タグをオープン状態に設定します。 |

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

「プロジェクト C」に関連するすべてのチェックボックス項目を完成させる方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
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

「プロジェクト C」に関連するすべてのチェックボックス項目を開く方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
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

不完全なチェックボックスでマークされ、先週作成されたアイテムを含むページを含む PDF を生成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
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

今週完了すべき Outlook の未完了タスクを含むページを含む PDF を生成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
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

### 関連項目

* interface [ITag](../itag/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


