---
title: Notebook.RemoveChild
second_title: Aspose.Note for .NET API リファレンス
description: Notebook 方法. 子ノードを削除します
type: docs
weight: 140
url: /ja/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

子ノードを削除します。

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| oldChild | INotebookChildNode | 削除するノード。 |

### 戻り値

削除されたノード。

### 例

ノートブックからすべてのセクションにアクセスする方法を示します。

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
```

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

ノートブックを保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### 関連項目

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* 名前空間 [Aspose.Note](../../notebook/)
* 組み立て [Aspose.Note](../../../)


