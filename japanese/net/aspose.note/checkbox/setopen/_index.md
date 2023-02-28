---
title: CheckBox.SetOpen
second_title: Aspose.Note for .NET API リファレンス
description: CheckBox 方法. タグをオープン状態に設定します
type: docs
weight: 80
url: /ja/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

タグをオープン状態に設定します。

```csharp
public virtual void SetOpen()
```

### 例

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

### 関連項目

* class [CheckBox](../)
* 名前空間 [Aspose.Note](../../checkbox/)
* 組み立て [Aspose.Note](../../../)


