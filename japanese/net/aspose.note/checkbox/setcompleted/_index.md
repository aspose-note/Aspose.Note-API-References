---
title: CheckBox.SetCompleted
second_title: Aspose.Note for .NET API リファレンス
description: CheckBox 方法. タグを完了状態に設定します
type: docs
weight: 70
url: /ja/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

タグを完了状態に設定します。

```csharp
public void SetCompleted(DateTime completedTime)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| completedTime | DateTime | 完了時間. |

### 関連項目

* class [CheckBox](../)
* 名前空間 [Aspose.Note](../../checkbox/)
* 組み立て [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

現在時刻を完了時刻としてタグを完了状態に設定します。

```csharp
public void SetCompleted()
```

### 例

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

### 関連項目

* class [CheckBox](../)
* 名前空間 [Aspose.Note](../../checkbox/)
* 組み立て [Aspose.Note](../../../)


