---
title: Document.DetectLayoutChanges
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. 前回の変更以降にドキュメント レイアウトに加えられたすべての変更を検出しますDetectLayoutChanges call. の場合AutomaticLayoutChangesDetectionEnabledドキュメント エクスポートの開始時に自動的に使用されるtrue に設定します
type: docs
weight: 90
url: /ja/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

前回の変更以降にドキュメント レイアウトに加えられたすべての変更を検出します。`DetectLayoutChanges` call. の場合[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/)ドキュメント エクスポートの開始時に自動的に使用される、true に設定します。

```csharp
public void DetectLayoutChanges()
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


