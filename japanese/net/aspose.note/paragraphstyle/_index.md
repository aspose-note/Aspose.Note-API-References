---
title: Class ParagraphStyle
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.ParagraphStyle クラス. 一致する TextStyle オブジェクトがない場合に使用されるテキスト スタイル設定Stylesコレクションかこのオブジェクトは必要な設定を指定していません.
type: docs
weight: 510
url: /ja/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

一致する TextStyle オブジェクトがない場合に使用されるテキスト スタイル設定Stylesコレクションか、このオブジェクトは必要な設定を指定していません.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | の新しいインスタンスを初期化します`ParagraphStyle`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | デフォルト設定の ParagraphStyle を取得します。 |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | フォントの色を取得または設定します。 |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | フォント名を取得または設定します。 |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | フォント サイズを取得または設定します。 |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | フォント スタイルを取得します。 |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | ハイライトの色を取得または設定します。 |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | テキスト スタイルが太字かどうかを示す値を取得または設定します。 |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | テキスト スタイルが斜体かどうかを示す値を取得または設定します。 |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | テキスト スタイルが取り消し線かどうかを示す値を取得または設定します。 |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | テキスト スタイルが下付きかどうかを示す値を取得または設定します。 |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | テキスト スタイルが上付きかどうかを示す値を取得または設定します。 |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | テキスト スタイルが下線かどうかを示す値を取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | タイプのハッシュ関数として機能します。 |

### 例

フォントのサイズを大きくして、他のヘッダーの中でもページのタイトルを強調しましょう。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Aspose.one");

// ページのタイトルを繰り返します。
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

ハイライトで最新のテキストの変更点を強調しましょう。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Aspose.one");

// 先週変更された RichText ノードを取得します。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // ハイライトの色を設定
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // ハイライトの色を設定
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

段落スタイルを使用してテキスト形式で操作します。

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

中国語の番号付けを使用して新しいリストを挿入する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote ドキュメントを初期化します
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote ページを初期化
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// テキストスタイル設定を適用
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 同じアウトライン内の数字は自動的にインクリメントされます。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

新しい箇条書きリストを挿入する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document クラスのオブジェクトを作成します
Aspose.Note.Document doc = new Aspose.Note.Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// TextStyle クラス オブジェクトを初期化し、書式設定プロパティを設定します
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement クラス オブジェクトを初期化し、箇条書きを適用する
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText クラス オブジェクトを初期化し、テキスト スタイルを適用します
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline ノードを追加
page.AppendChildLast(outline);
// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

番号付けされた新しいリストを挿入する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// TextStyle クラス オブジェクトを初期化し、書式設定プロパティを設定します
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement クラス オブジェクトを初期化し、番号付けを適用します
// 同じアウトライン内の数字は自動的にインクリメントされます。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### 関連項目

* class [Style](../style/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


