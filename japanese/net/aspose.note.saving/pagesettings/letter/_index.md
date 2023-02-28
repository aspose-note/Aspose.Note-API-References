---
title: PageSettings.Letter
second_title: Aspose.Note for .NET API リファレンス
description: PageSettings 財産. レター形式ページの設定を取得します
type: docs
weight: 30
url: /ja/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

レター形式ページの設定を取得します。

```csharp
public static PageSettings Letter { get; }
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

### 関連項目

* class [PageSettings](../)
* 名前空間 [Aspose.Note.Saving](../../pagesettings/)
* 組み立て [Aspose.Note](../../../)


