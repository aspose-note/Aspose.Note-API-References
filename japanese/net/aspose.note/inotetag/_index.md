---
title: Interface INoteTag
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.INoteTag インターフェース. メモ タグ つまりOutlook タスクに関連付けられていないタグ のインターフェイス
type: docs
weight: 180
url: /ja/net/aspose.note/inotetag/
---
## INoteTag interface

メモ タグ (つまり、Outlook タスクに関連付けられていないタグ) のインターフェイス。

```csharp
public interface INoteTag : ITag
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | フォントの色を取得または設定します。 |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | ハイライトの色を取得または設定します。 |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | ラベル テキストを取得または設定します。 |

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

* interface [ITag](../itag/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


