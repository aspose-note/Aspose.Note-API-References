---
title: Class RichText
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.RichText クラス. リッチ テキストを表します
type: docs
weight: 530
url: /ja/net/aspose.note/richtext/
---
## RichText class

リッチ テキストを表します。

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [RichText](richtext/#constructor)() | の新しいインスタンスを初期化します`RichText`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | 配置を取得または設定します。 |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | このノードが複合かどうかを示す値を取得します。 true の場合、ノードは子ノードを持つことができます。 |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |
| [Length](../../aspose.note/richtext/length/) { get; } | テキストの長さを取得します。 |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | 行間隔を取得または設定します。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | 段落スタイルを取得または設定します。 これらの設定は、一致する TextStyle オブジェクトがStylesコレクションか、このオブジェクトは必要な設定を指定していません. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | 後のスペースの最小量を取得または設定します。 |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | 前のスペースの最小量を取得または設定します。 |
| [Tags](../../aspose.note/richtext/tags/) { get; } | 段落のすべてのタグのリストを取得します。 |
| [Text](../../aspose.note/richtext/text/) { get; set; } | テキストを取得または設定します。文字列には、値 10 (改行). の文字を含めてはなりません。 |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | テキスト ランのコレクションを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |
| [Append](../../aspose.note/richtext/append/#append)(string) | 最後のテキスト範囲に文字列を追加します。 |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | 末尾に文字列を追加します。 |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | 最初のテキスト範囲の先頭に文字列を追加します。 |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | 先頭に文字列を追加します。 |
| [Clear](../../aspose.note/richtext/clear/)() | このインスタンスのコンテンツをクリアします。 |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | この RichText オブジェクトの文字を反復処理する列挙子を返します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | この文字列で指定された Unicode 文字が最初に出現した位置のゼロから始まるインデックスを返します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | このインスタンスで指定された文字列が最初に出現した位置の 0 から始まるインデックスを返します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | この文字列で指定された Unicode 文字が最初に出現した位置のゼロから始まるインデックスを返します。指定した文字位置から検索を開始します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | このインスタンスで指定された文字列が最初に出現した位置のゼロから始まるインデックスを返します。指定した文字位置から検索を開始します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | 現在のインスタンスで指定された文字列が最初に出現した位置の 0 から始まるインデックスを返します。パラメーターは、指定された文字列に使用する検索の種類を指定します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | このインスタンスで指定された文字が最初に出現した位置のゼロから始まるインデックスを返します。指定した文字位置から検索を開始し、指定した数の文字位置を調べます。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | このインスタンスで指定された文字列が最初に出現した位置のゼロから始まるインデックスを返します。指定した文字位置から検索を開始し、指定した数の文字位置を調べます。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | 現在のインスタンスで指定された文字列が最初に出現した位置の 0 から始まるインデックスを返します。パラメーターは、現在の文字列内の検索開始位置と、指定された文字列に使用する検索の種類を指定します。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | 現在のインスタンスで指定された文字列が最初に出現した位置の 0 から始まるインデックスを返します。 |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | このインスタンスの指定されたインデックス位置に指定された文字列を挿入します。 |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | このインスタンスの指定されたインデックス位置に、指定されたスタイルで指定された文字列を挿入します。 |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | 現在のインスタンス内の指定された位置から最後の位置までのすべての文字を削除します。 |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | 現在のインスタンスの指定された位置から指定された数の文字を削除します。 |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | このインスタンスで出現する指定された Unicode 文字をすべて、指定された別の Unicode 文字に置き換えます。 |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | 現在のインスタンス内の指定された文字列のすべてのオカレンスを別の指定された文字列に置き換えます。 |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | 現在のインスタンスで出現する指定された文字列をすべて、指定されたスタイルの別の指定された文字列に置き換えます。 |
| [Trim](../../aspose.note/richtext/trim/#trim)() | 前後の空白文字をすべて削除します。 |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | 文字の先頭および末尾のインスタンスをすべて削除します。 |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | 配列で指定された一連の文字の先頭および末尾のオカレンスをすべて削除します。 |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | 末尾の空白文字をすべて削除します。 |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | 後続の文字をすべて削除します。 |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | 配列で指定された一連の文字の末尾の出現をすべて削除します。 |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | 先頭の空白文字をすべて削除します。 |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | 指定された文字の先頭の出現箇所をすべて削除します。 |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | 配列で指定された一連の文字の先頭の出現箇所をすべて削除します。 |

### 例

ドキュメントからすべてのテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// テキストを取得
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// 出力画面にテキストを出力
Console.WriteLine(text);
```

ページからすべてのテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// ページノードのリストを取得
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // テキストを取得
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // 出力画面にテキストを出力
    Console.WriteLine(text);
}
```

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

すべてのテーブルの行からテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tables();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Sample1.one");

// テーブル ノードのリストを取得します
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 表の行を繰り返します
    foreach (TableRow row in table)
    {
        // テキストを取得
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 出力画面にテキストを出力
        Console.WriteLine(text);
    }
}
```

テーブルからテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tables();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Sample1.one");

// テーブル ノードのリストを取得します
IList<Table> nodes = document.GetChildNodes<Table>();

// テーブル数を設定
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // テキストを取得
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // 出力画面にテキストを出力
    Console.WriteLine(text);
}
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

ページのタイトルを設定する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
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

すべてのページを通過し、テキストを置換する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての RichText ノードを取得します
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 図形のテキストを置き換える
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// サポートされている任意のファイル形式に保存
oneFile.Save(dataDir, SaveFormat.Pdf);
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

表のセルからテキストを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tables();

// ドキュメントを Aspose.Note にロードします。
Document document = new Document(dataDir + "Sample1.one");

// テーブル ノードのリストを取得します
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 表の行を繰り返します
    foreach (TableRow row in table)
    {
        // TableCell ノードのリストを取得
        // 表のセルを繰り返します
        foreach (TableCell cell in row)
        {
            // テキストを取得
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 出力画面にテキストを出力
            Console.WriteLine(text);
        }
    }
}
```

ページのテキストを通過させて置換する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// すべての RichText ノードを取得します
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 図形のテキストを置き換える
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// サポートされている任意のファイル形式に保存
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

ドキュメントを作成し、デフォルト オプションを使用して HTML 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote ドキュメントを初期化します
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// ドキュメント内のすべてのテキストのデフォルト スタイル。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// HTML形式で保存
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

タグを使用して新しい段落を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// テキストノードを追加
outlineElem.AppendChildLast(text);

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

ドキュメントを作成し、指定した範囲のページを html 形式で保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote ドキュメントを初期化します
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// ドキュメント内のすべてのテキストのデフォルト スタイル。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML形式で保存
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

タグの詳細にアクセスする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "TagFile.one");

// すべての RichText ノードを取得します
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 各ノードを繰り返します
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // プロパティを取得する
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

テキストを含むドキュメントを作成する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Page page = new Page(doc);

// Outline クラス オブジェクトの初期化
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle クラス オブジェクトを初期化し、書式設定プロパティを設定します
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText クラス オブジェクトを初期化し、テキスト スタイルを適用します
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText ノードを追加
outlineElem.AppendChildLast(text);

// OutlineElement ノードを追加
outline.AppendChildLast(outlineElem);

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

毎週のミーティングのテンプレートを準備する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// Document クラスのオブジェクトを作成します
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


