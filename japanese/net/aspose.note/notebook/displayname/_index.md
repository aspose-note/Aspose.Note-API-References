---
title: Notebook.DisplayName
second_title: Aspose.Note for .NET API リファレンス
description: Notebook 財産. 表示名を取得または設定します
type: docs
weight: 40
url: /ja/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

表示名を取得または設定します。

```csharp
public string DisplayName { get; set; }
```

### 例

ノートブックからセクションを削除する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "test.onetoc2");

// その子ノードをトラバースして、目的の子アイテムを検索します
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // ノートブックから子アイテムを削除します
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// ノートブックを保存します
notebook.Save(dataDir);
```

### 関連項目

* class [Notebook](../)
* 名前空間 [Aspose.Note](../../notebook/)
* 組み立て [Aspose.Note](../../../)


