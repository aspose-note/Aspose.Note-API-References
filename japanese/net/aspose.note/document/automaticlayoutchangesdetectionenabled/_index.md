---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note for .NET API リファレンス
description: Document 財産. Aspose.Note がレイアウト変更の検出を自動的に実行するかどうかを示す値を取得または設定します デフォルト値は真実.
type: docs
weight: 20
url: /ja/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Aspose.Note がレイアウト変更の検出を自動的に実行するかどうかを示す値を取得または設定します。 デフォルト値は`真実`.

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### 例

ドキュメントをさまざまな形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 新しいドキュメントを初期化します
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 新しいページを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// ドキュメント内のすべてのテキストのデフォルト スタイル。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントをさまざまな形式で保存し、テキストのフォント サイズを設定し、レイアウトの変更を手動で検出します。
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### 関連項目

* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


