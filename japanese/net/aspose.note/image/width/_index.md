---
title: Image.Width
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 幅を取得または設定しますこれはMS OneNote ドキュメント内の画像の実際の幅です.
type: docs
weight: 180
url: /ja/net/aspose.note/image/width/
---
## Image.Width property

幅を取得または設定します。これは、MS OneNote ドキュメント内の画像の実際の幅です.

```csharp
public float Width { get; set; }
```

### 例

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


