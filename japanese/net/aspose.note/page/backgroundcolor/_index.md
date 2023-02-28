---
title: Page.BackgroundColor
second_title: Aspose.Note for .NET API リファレンス
description: Page 財産. ページの背景色を取得または設定します
type: docs
weight: 30
url: /ja/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

ページの背景色を取得または設定します。

```csharp
public Color BackgroundColor { get; set; }
```

### 例

ページの背景色を設定する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

ドキュメントにダーク テーマ スタイルを適用する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### 関連項目

* class [Page](../)
* 名前空間 [Aspose.Note](../../page/)
* 組み立て [Aspose.Note](../../../)


