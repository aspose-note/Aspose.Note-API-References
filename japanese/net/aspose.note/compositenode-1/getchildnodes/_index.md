---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note for .NET API リファレンス
description: CompositeNode 方法. ノード タイプ別にすべての子ノードを取得します
type: docs
weight: 70
url: /ja/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

ノード タイプ別にすべての子ノードを取得します。

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| パラメータ | 説明 |
| --- | --- |
| T1 | 返されたリスト内の要素の型。 |

### 戻り値

子ノードのリスト。

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* 名前空間 [Aspose.Note](../../compositenode-1/)
* 組み立て [Aspose.Note](../../../)


