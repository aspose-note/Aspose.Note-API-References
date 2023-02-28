---
title: Class NotebookLoadOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.NotebookLoadOptions クラス. ノートブックの読み込みに使用されるオプション
type: docs
weight: 420
url: /ja/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

ノートブックの読み込みに使用されるオプション。

```csharp
public class NotebookLoadOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | 子ドキュメント を後で明示的にロードする必要があるかどうかを示す値を取得または設定します. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | 親ドキュメントのロード中に子ドキュメント をロードする必要があるかどうかを示す値を取得または設定します。 |

### 例

ノートブックを暗号化する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


