---
title: Class PageSettings
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.PageSettings クラス. ページのレイアウト設定を表します
type: docs
weight: 820
url: /ja/net/aspose.note.saving/pagesettings/
---
## PageSettings class

ページのレイアウト設定を表します。

```csharp
public class PageSettings
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | A4 形式のページの設定を取得します。 |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | 高さ制限のない A4 形式のページの設定を取得します。 |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | レター形式ページの設定を取得します。 |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | 高さ制限なしのレター形式ページの設定を取得します。 |

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

* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


