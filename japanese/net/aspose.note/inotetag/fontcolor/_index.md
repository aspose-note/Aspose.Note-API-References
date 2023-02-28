---
title: INoteTag.FontColor
second_title: Aspose.Note for .NET API リファレンス
description: INoteTag 財産. フォントの色を取得または設定します
type: docs
weight: 10
url: /ja/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

フォントの色を取得または設定します。

```csharp
public Color FontColor { get; set; }
```

### 例

タグの詳細にアクセスする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Tags();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "TagFile.one");

// すべての RichText ノードを取得します
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 各ノードを繰り返します
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // プロパティを取得する
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### 関連項目

* interface [INoteTag](../)
* 名前空間 [Aspose.Note](../../inotetag/)
* 組み立て [Aspose.Note](../../../)


