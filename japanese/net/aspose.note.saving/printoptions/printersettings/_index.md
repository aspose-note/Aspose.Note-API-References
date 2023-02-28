---
title: PrintOptions.PrinterSettings
second_title: Aspose.Note for .NET API リファレンス
description: PrintOptions 財産. プリンター設定を取得または設定します
type: docs
weight: 40
url: /ja/net/aspose.note.saving/printoptions/printersettings/
---
## PrintOptions.PrinterSettings property

プリンター設定を取得または設定します。

```csharp
public PrinterSettings PrinterSettings { get; set; }
```

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

* class [PrintOptions](../)
* 名前空間 [Aspose.Note.Saving](../../printoptions/)
* 組み立て [Aspose.Note](../../../)


