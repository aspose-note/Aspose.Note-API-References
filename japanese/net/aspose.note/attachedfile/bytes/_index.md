---
title: AttachedFile.Bytes
second_title: Aspose.Note for .NET API リファレンス
description: AttachedFile 財産. 埋め込みファイルのバイナリ データを取得します
type: docs
weight: 50
url: /ja/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

埋め込みファイルのバイナリ データを取得します。

```csharp
public byte[] Bytes { get; }
```

### 例

添付ファイルのコンテンツを取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Attachments();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Sample1.one");

// 添付ファイル ノードのリストを取得します
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// すべてのノードを繰り返します
foreach (AttachedFile file in nodes)
{
    // ストリームオブジェクトに添付ファイルをロード
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // ローカル ファイルを作成します
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // ファイルストリームをコピー
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### 関連項目

* class [AttachedFile](../)
* 名前空間 [Aspose.Note](../../attachedfile/)
* 組み立て [Aspose.Note](../../../)


