---
title: Image.OriginalHeight
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 元の高さを取得しますこれはサイズ変更前の画像の元の幅です
type: docs
weight: 140
url: /ja/net/aspose.note/image/originalheight/
---
## Image.OriginalHeight property

元の高さを取得します。これは、サイズ変更前の画像の元の幅です。

```csharp
public float OriginalHeight { get; }
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

### 関連項目

* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


