---
title: Class PrintOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.PrintOptions クラス. ドキュメントの印刷に使用されるオプション
type: docs
weight: 860
url: /ja/net/aspose.note.saving/printoptions/
---
## PrintOptions class

ドキュメントの印刷に使用されるオプション。

```csharp
public class PrintOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [PrintOptions](printoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | ドキュメントの印刷中に (たとえば、印刷ステータス ダイアログ ボックスやプリンター キューに) 表示するドキュメント名を取得または設定します。 |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | ページ分割に使用されるアルゴリズムを取得または設定します。 |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | プリンター設定を取得または設定します。 |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | 生成された画像の解像度を 1 インチあたりのドット数で取得または設定します。 |

### 例

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

### 関連項目

* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


