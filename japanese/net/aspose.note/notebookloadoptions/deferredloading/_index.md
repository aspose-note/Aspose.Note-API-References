---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note for .NET API リファレンス
description: NotebookLoadOptions 財産. 子ドキュメント を後で明示的にロードする必要があるかどうかを示す値を取得または設定します.
type: docs
weight: 20
url: /ja/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

子ドキュメント を後で明示的にロードする必要があるかどうかを示す値を取得または設定します.

```csharp
public bool DeferredLoading { get; set; }
```

### 備考

デフォルト値は`間違い`であるため、子ドキュメントは暗黙的にロードされます。 値`真実`ユーザーが電話する必要があることを示しています[`LoadChildDocument`](../../notebook/loadchilddocument/)また ノートブック自体がロードされた後の各ノートブックの子ノード。 値が`真実`、[`InstantLoading`](../instantloading/)オプションは無視されます。 ノートブックがストリームからロードされている場合、値は常に`真実`ユーザーによって明示的に設定されていたにもかかわらず`間違い`.

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

* class [NotebookLoadOptions](../)
* 名前空間 [Aspose.Note](../../notebookloadoptions/)
* 組み立て [Aspose.Note](../../../)


