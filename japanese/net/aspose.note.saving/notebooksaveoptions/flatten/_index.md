---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note for .NET API リファレンス
description: NotebookSaveOptions 財産. ノートブックの子階層がフラット化されて保存されるかどうかを示す値を取得または設定します
type: docs
weight: 20
url: /ja/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

ノートブックの子階層がフラット化されて保存されるかどうかを示す値を取得または設定します。

```csharp
public bool Flatten { get; set; }
```

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

* class [NotebookSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../notebooksaveoptions/)
* 組み立て [Aspose.Note](../../../)


