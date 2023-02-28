---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.NotebookPdfSaveOptions クラス. ノートブック ページを PDF にレンダリングするときに追加オプションを指定できます
type: docs
weight: 780
url: /ja/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

ノートブック ページを PDF にレンダリングするときに追加オプションを指定できます。

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | 子ドキュメント を明示的に保存する必要があるかどうかを示す値を取得または設定します. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | ノートブックの子階層がフラット化されて保存されるかどうかを示す値を取得または設定します。 |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


