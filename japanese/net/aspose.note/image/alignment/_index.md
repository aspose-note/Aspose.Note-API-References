---
title: Image.Alignment
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 配置を取得または設定します
type: docs
weight: 20
url: /ja/net/aspose.note/image/alignment/
---
## Image.Alignment property

配置を取得または設定します。

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### 例

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

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


