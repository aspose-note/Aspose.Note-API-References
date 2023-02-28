---
title: Image.HyperlinkUrl
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 画像に関連付けられたハイパーリンクを取得または設定します
type: docs
weight: 110
url: /ja/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

画像に関連付けられたハイパーリンクを取得または設定します。

```csharp
public string HyperlinkUrl { get; set; }
```

### 例

ハイパーリンクを画像にバインドする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### 関連項目

* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


