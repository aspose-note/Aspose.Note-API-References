---
title: Class TextStyle
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.TextStyle クラス. 文字スタイルを指定します
type: docs
weight: 970
url: /ja/net/aspose.note/textstyle/
---
## TextStyle class

文字スタイルを指定します。

```csharp
public sealed class TextStyle : Style
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [TextStyle](textstyle/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | 「en-US」カルチャでスタイルを取得します。 |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | MS OneNote のタイトル日付のデフォルト スタイルを取得します。 |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | MS OneNote のタイトル テキストのデフォルト スタイルを取得します。 |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | MS OneNote のタイトル時間のデフォルト スタイルを取得します。 |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | フォントの色を取得または設定します。 |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | フォント名を取得または設定します。 |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | フォント サイズを取得または設定します。 |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | フォント スタイルを取得します。 |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | ハイライトの色を取得または設定します。 |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | ハイパーリンク アドレスを取得または設定します。の値が[`IsHyperlink`](./ishyperlink/)プロパティは true. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | テキスト スタイルが太字かどうかを示す値を取得または設定します。 |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | テキスト スタイルが非表示かどうかを示す値を取得または設定します。 |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | テキスト スタイルがハイパーリンクかどうかを示す値を取得または設定します。 |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | テキスト スタイルが斜体かどうかを示す値を取得または設定します。 |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | テキスト スタイルが数学形式かどうかを示す値を取得または設定します。 |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | テキスト スタイルが取り消し線かどうかを示す値を取得または設定します。 |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | テキスト スタイルが下付きかどうかを示す値を取得または設定します。 |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | テキスト スタイルが上付きかどうかを示す値を取得または設定します。 |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | テキスト スタイルが下線かどうかを示す値を取得または設定します。 |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | テキストの言語を取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | タイプのハッシュ関数として機能します。 |

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

テキストの校正言語を設定します。

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

ハイパーリンクをテキストにバインドする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tasks();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem);

// タイトル クラス オブジェクトを初期化します
Title title = new Title() { TitleText = titleText };

// Page クラス オブジェクトを初期化します
Page page = new Note.Page() { Title = title };

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### 関連項目

* class [Style](../style/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


