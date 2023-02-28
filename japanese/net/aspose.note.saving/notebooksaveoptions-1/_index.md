---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions クラス. 特定の format のノートブック保存オプションを表しすべてのドキュメントの子ノードに共通の保存オプションを提供する抽象基本クラス.
type: docs
weight: 800
url: /ja/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

特定の format のノートブック保存オプションを表し、すべてのドキュメントの子ノードに共通の保存オプションを提供する抽象基本クラス.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| パラメータ | 説明 |
| --- | --- |
| TDocumentSaveOptions | すべてのノートブックの子ドキュメントの保存オプション. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 子ドキュメント を明示的に保存する必要があるかどうかを示す値を取得または設定します. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | すべてのノートブックの子ドキュメントの保存オプションを取得または設定します. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | ノートブックの子階層がフラット化されて保存されるかどうかを示す値を取得または設定します。 |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | ノートブックの保存形式を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | すべてのノートブックの子ドキュメントの保存オプションを取得します. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


