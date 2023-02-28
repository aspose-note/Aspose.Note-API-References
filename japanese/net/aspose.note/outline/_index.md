---
title: Class Outline
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Outline クラス. アウトラインを表します
type: docs
weight: 450
url: /ja/net/aspose.note/outline/
---
## Outline class

アウトラインを表します。

```csharp
public sealed class Outline : IndentatedNode<IOutlineChildNode>, IPageChildNode
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Outline](outline/#constructor)() | の新しいインスタンスを初期化します`Outline`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved/) { get; set; } | アウトラインの子孫を移動できるかどうかを取得します. |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset/) { get; set; } | 水平オフセットを取得または設定します。 |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |
| [MaxHeight](../../aspose.note/outline/maxheight/) { get; set; } | 最大の高さを取得または設定します。 |
| [MaxWidth](../../aspose.note/outline/maxwidth/) { get; set; } | 最大幅を取得または設定します。 |
| [MinWidth](../../aspose.note/outline/minwidth/) { get; set; } | 最小幅を取得または設定します。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |
| [ReservedWidth](../../aspose.note/outline/reservedwidth/) { get; set; } | 予約された幅を取得または設定します。 |
| [VerticalOffset](../../aspose.note/outline/verticaloffset/) { get; set; } | 垂直オフセットを取得または設定します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### 例

タグ付きの新しい画像を追加する方法を示します。

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

// 画像を読み込む
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// ドキュメントノードに画像を挿入
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// アウトライン要素ノードを追加
outline.AppendChildLast(outlineElem);

// アウトラインノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "AddImageNodeWithTag_out.one";
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

### 関連項目

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


