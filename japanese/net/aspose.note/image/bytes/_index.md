---
title: Image.Bytes
second_title: Aspose.Note for .NET API リファレンス
description: Image 財産. 画像データ ストアを取得します
type: docs
weight: 50
url: /ja/net/aspose.note/image/bytes/
---
## Image.Bytes property

画像データ ストアを取得します。

```csharp
public byte[] Bytes { get; }
```

### 例

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

### 関連項目

* class [Image](../)
* 名前空間 [Aspose.Note](../../image/)
* 組み立て [Aspose.Note](../../../)


