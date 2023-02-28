---
title: Class PdfSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.PdfSaveOptions クラス. ドキュメント ページを PDF にレンダリングするときに追加オプションを指定できます
type: docs
weight: 850
url: /ja/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

ドキュメント ページを PDF にレンダリングするときに追加オプションを指定できます。

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 保存中に使用されるフォントの設定を取得または設定します |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | PDF ファイル内の画像に適用される圧縮の種類を取得または設定します。 |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | PDF ドキュメント内の JPEG 画像の品質を決定する値を取得または設定します。 値は 0 から 100 までの範囲で変化する場合があります。0 は最悪の品質ですが最大の圧縮率を意味し、100 は最高の品質ですが最小の圧縮率を意味します. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 保存するページ数を取得または設定します。デフォルトではMaxValue は、ドキュメントのすべてのページがレンダリングされることを意味します. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 保存する最初のページのインデックスを取得または設定します。デフォルトは 0. です |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | ドキュメント内の各ページのページ設定を取得または設定します。 デフォルトでは、CurrentUICulture に依存します。*US カルチャにはレター設定があり、その他には A4 設定があります。 |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | ページ分割に使用されるアルゴリズムを取得または設定します。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | ドキュメントの保存形式を取得します。 |

### 例

ドキュメントをレター ページ レイアウトの Pdf 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// ドキュメントを保存します。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

高さ制限のない A4 ページ レイアウトの Pdf 形式でドキュメントを保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// ドキュメントを保存します。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

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

長い OneNote ページを pdf 形式で保存すると、複数のページに分割されます。このサンプルは、ページの区切りにあるオブジェクトの分割ロジックを構成する方法を示しています。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

ドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions オブジェクトを初期化します
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 保存する最初のページのページ インデックスを設定します
                              PageIndex = 0,

                              // ページ数を設定
                              PageCount = 1,
                          };

// ドキュメントを PDF として保存
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

特定の設定を使用してドキュメントを PDF 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions オブジェクトを初期化します
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // JPEG 圧縮を使用
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 圧縮の品質
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

長い OneNote ページを pdf 形式で保存すると、複数のページに分割されます。この例は、ページの区切りにあるオブジェクトの分割ロジックを構成する方法を示しています。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// また
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### 関連項目

* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


