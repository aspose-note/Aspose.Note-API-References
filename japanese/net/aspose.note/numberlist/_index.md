---
title: Class NumberList
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.NumberList クラス. 番号付きまたは箇条書きのリストを表します
type: docs
weight: 440
url: /ja/net/aspose.note/numberlist/
---
## NumberList class

番号付きまたは箇条書きのリストを表します。

```csharp
public class NumberList
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | の新しいインスタンスを初期化します`NumberList`class. このインスタンスは箇条書きを表します。 |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | の新しいインスタンスを初期化します`NumberList` class. このインスタンスは番号付きリストを表します. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | フォントの名前を取得または設定します。 |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | フォントの色を取得または設定します。 |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | フォント サイズを取得または設定します。 |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | 行ヘッダーの形式を取得または設定します。箇条書きの場合、箇条書き記号を表します. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | テキスト スタイルが太字かどうかを示す値を取得または設定します。 |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | テキスト スタイルが斜体かどうかを示す値を取得または設定します。 |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | 自動的に番号付けされたオブジェクトのグループに使用される数値形式を取得または設定します。箇条書きの場合は null にする必要があります。 |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | リスト アイテムの自動数値を上書きする数値を取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | タイプのハッシュ関数として機能します。 |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | 番号付きリスト ヘッダーを取得します。 |

### 例

リストの書式設定に関する情報を取得する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// アウトライン要素のコレクション ノードを取得します
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 各ノードを繰り返します
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // フォント名を取得
        Console.WriteLine("Font Name: " + list.Font);

        // フォントの長さを取得
        Console.WriteLine("Font Length: " + list.Font.Length);

        // フォントサイズを取得
        Console.WriteLine("Font Size: " + list.FontSize);

        // フォントの色を取得
        Console.WriteLine("Font Color: " + list.FontColor);

        // フォーマットを取得
        Console.WriteLine("Font format: " + list.Format);

        //太字にチェック
        Console.WriteLine("Is bold: " + list.IsBold);

        // 斜体にチェック
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


