---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note for .NET API リファレンス
description: ImageSaveOptions 財産. 生成された画像の解像度を 1 インチあたりのドット数で取得または設定します
type: docs
weight: 50
url: /ja/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

生成された画像の解像度を 1 インチあたりのドット数で取得または設定します。

```csharp
public float Resolution { get; set; }
```

### 備考

デフォルト値は 96 です。

### 例

ドキュメントを画像として保存するときに画像の解像度を設定する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// ドキュメントを保存します。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
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

* class [ImageSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../imagesaveoptions/)
* 組み立て [Aspose.Note](../../../)


