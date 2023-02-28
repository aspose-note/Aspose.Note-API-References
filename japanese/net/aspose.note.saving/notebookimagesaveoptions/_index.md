---
title: Class NotebookImageSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.NotebookImageSaveOptions クラス. ノートブックのページを画像にレンダリングする際に追加オプションを指定できます.
type: docs
weight: 760
url: /ja/net/aspose.note.saving/notebookimagesaveoptions/
---
## NotebookImageSaveOptions class

ノートブックのページを画像にレンダリングする際に追加オプションを指定できます.

```csharp
public class NotebookImageSaveOptions : NotebookSaveOptions<ImageSaveOptions>
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [NotebookImageSaveOptions](notebookimagesaveoptions/)(SaveFormat) | の新しいインスタンスを初期化します`NotebookImageSaveOptions`class. |

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

フラット化されたノートブックを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// ノートブックを保存します
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

指定したオプションを使用してノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
```

フラット化されたノートブックを画像として保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote ノートブックを読み込む
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// ノートブックを保存します
notebook.Save(dataDir, notebookSaveOptions);
```

### 関連項目

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [ImageSaveOptions](../imagesaveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


