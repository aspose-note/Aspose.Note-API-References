---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm クラス. 元のページに収まらない場合はオブジェクト全体を次のページに移動します
type: docs
weight: 740
url: /ja/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

元のページに収まらない場合は、オブジェクト全体を次のページに移動します。

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | の新しいインスタンスを初期化します`KeepSolidObjectsAlgorithm`複製されたパーツのデフォルトの高さ制限を使用するクラス. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | の新しいインスタンスを初期化します`KeepSolidObjectsAlgorithm`複製されたパーツの特定の高さ制限を使用するクラス. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | 複製パーツの高さ制限を取得します。 |

## 田畑

| 名前 | 説明 |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | 複製されたパーツのデフォルトの最大サイズ. |

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

オプションを指定して標準の Windows ダイアログを使用して、ドキュメントをプリンターに送信する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


