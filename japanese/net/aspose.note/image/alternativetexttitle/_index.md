---
title: Image.AlternativeTextTitle
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 画像の代替テキストのタイトルを取得または設定します
type: docs
weight: 40
url: /ja/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

画像の代替テキストのタイトルを取得または設定します。

```csharp
public string AlternativeTextTitle { get; set; }
```

### 例

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

### 関連項目

* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


