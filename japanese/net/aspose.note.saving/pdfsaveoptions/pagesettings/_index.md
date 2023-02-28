---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note for .NET API リファレンス
description: PdfSaveOptions 財産. ドキュメント内の各ページのページ設定を取得または設定します デフォルトではCurrentUICulture に依存しますUS カルチャにはレター設定がありその他には A4 設定があります
type: docs
weight: 40
url: /ja/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

ドキュメント内の各ページのページ設定を取得または設定します。 デフォルトでは、CurrentUICulture に依存します。*US カルチャにはレター設定があり、その他には A4 設定があります。

```csharp
public PageSettings PageSettings { get; set; }
```

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

### 関連項目

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 組み立て [Aspose.Note](../../../)


