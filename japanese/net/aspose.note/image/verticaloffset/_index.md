---
title: Image.VerticalOffset
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 垂直オフセットを取得または設定します
type: docs
weight: 170
url: /ja/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

垂直オフセットを取得または設定します。

```csharp
public float VerticalOffset { get; set; }
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

### 関連項目

* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


