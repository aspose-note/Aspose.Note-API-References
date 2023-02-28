---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: NotebookSaveOptions 財産. すべてのノートブックの子ドキュメントの保存オプションを取得または設定します.
type: docs
weight: 10
url: /ja/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

すべてのノートブックの子ドキュメントの保存オプションを取得または設定します.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### 例

指定したオプションを使用してノートブックを pdf 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
```

### 関連項目

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* 名前空間 [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* 組み立て [Aspose.Note](../../../)


