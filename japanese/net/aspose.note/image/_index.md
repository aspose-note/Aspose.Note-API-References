---
title: Class Image
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Image クラス. は画像を表します.
type: docs
weight: 250
url: /ja/net/aspose.note/image/
---
## Image class

は画像を表します.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Image](image/#constructor)() | の新しいインスタンスを初期化します`Image`class. |
| [Image](image/#constructor_4)(string, Stream) | の新しいインスタンスを初期化します`Image`class. |
| [Image](image/#constructor_5)(string, string, string) | の新しいインスタンスを初期化します`Image`class. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | 配置を取得または設定します。 |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | 画像の本文と代替テキストを取得または設定します。 |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | 画像の代替テキストのタイトルを取得または設定します。 |
| [Bytes](../../aspose.note/image/bytes/) { get; } | 画像データ ストアを取得します。 |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| [FileName](../../aspose.note/image/filename/) { get; } | ファイル名を取得します。 |
| [FilePath](../../aspose.note/image/filepath/) { get; } | 画像ファイルへのパスを取得します。 |
| [Format](../../aspose.note/image/format/) { get; } | 画像のフォーマットを取得します. |
| [Height](../../aspose.note/image/height/) { get; set; } | 高さを取得または設定します。これは、MS OneNote ドキュメント内の画像の実際の高さです. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | 水平オフセットを取得または設定します。 |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | 画像に関連付けられたハイパーリンクを取得または設定します。 |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | 画像が背景画像かどうかを取得します。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | このノードが複合かどうかを示す値を取得します。 true の場合、ノードは子ノードを持つことができます。 |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | 元の高さを取得します。これは、サイズ変更前の画像の元の幅です。 |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | 元の幅を取得します。これは、サイズ変更前の画像の元の幅です。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |
| [Tags](../../aspose.note/image/tags/) { get; } | 段落のすべてのタグのリストを取得します。 |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | 垂直オフセットを取得または設定します。 |
| [Width](../../aspose.note/image/width/) { get; set; } | 幅を取得または設定します。これは、MS OneNote ドキュメント内の画像の実際の幅です. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |

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

画像のテキスト説明を設定する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

ドキュメントから画像を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての画像ノードを取得
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // 画像バイトをファイルに保存します
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

画像のメタ情報を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

// すべての画像ノードを取得
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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

ユーザー定義のプロパティを使用して、ファイルからドキュメントに画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// ストリームからドキュメントを読み込みます。
Document doc = new Document(dataDir + "Aspose.one");

// ドキュメントの最初のページを取得します。
Aspose.Note.Page page = doc.FirstChild;

// ファイルから画像を読み込みます。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 必要に応じて画像のサイズを変更します (オプション)。
                              Width = 100,
                              Height = 100,

                              // ページ内の画像の位置を設定します (オプション)。
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // 画像の配置を設定
                              Alignment = HorizontalAlignment.Right
                          };

// ページに画像を追加します。
page.AppendChildLast(image);
```

ストリームからドキュメントに画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // イメージ名、拡張子、およびストリームを使用して 2 番目のイメージをロードします。
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // 画像の配置を設定
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

ファイルからドキュメントに画像を追加する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Images();

// Document クラスのオブジェクトを作成します
Document doc = new Document();

// Page クラス オブジェクトを初期化します
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline クラス オブジェクトを初期化し、オフセット プロパティを設定します
Outline outline = new Outline(doc);

// OutlineElement クラス オブジェクトを初期化します
OutlineElement outlineElem = new OutlineElement(doc);

// ファイル パスで画像を読み込みます。
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // 画像の配置を設定
                              Alignment = HorizontalAlignment.Right
                          };

// 画像を追加
outlineElem.AppendChildLast(image);

// アウトライン要素を追加
outline.AppendChildLast(outlineElem);

// Outline ノードを追加
page.AppendChildLast(outline);

// ページノードを追加
doc.AppendChildLast(page);

// OneNote ドキュメントを保存
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### 関連項目

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


