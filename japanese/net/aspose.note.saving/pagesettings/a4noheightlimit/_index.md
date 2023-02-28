---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note for .NET API リファレンス
description: PageSettings 財産. 高さ制限のない A4 形式のページの設定を取得します
type: docs
weight: 20
url: /ja/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

高さ制限のない A4 形式のページの設定を取得します。

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### 例

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

* class [PageSettings](../)
* 名前空間 [Aspose.Note.Saving](../../pagesettings/)
* 組み立て [Aspose.Note](../../../)


