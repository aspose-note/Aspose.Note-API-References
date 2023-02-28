---
title: NumberList.IsItalic
second_title: Aspose.Note for .NET API リファレンス
description: NumberList 財産. テキスト スタイルが斜体かどうかを示す値を取得または設定します
type: docs
weight: 70
url: /ja/net/aspose.note/numberlist/isitalic/
---
## NumberList.IsItalic property

テキスト スタイルが斜体かどうかを示す値を取得または設定します。

```csharp
public bool IsItalic { get; set; }
```

### 例

リストの書式設定に関する情報を取得する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// アウトライン要素のコレクション ノードを取得します
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 各ノードを繰り返します
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // フォント名を取得
        Console.WriteLine("Font Name: " + list.Font);

        // フォントの長さを取得
        Console.WriteLine("Font Length: " + list.Font.Length);

        // フォントサイズを取得
        Console.WriteLine("Font Size: " + list.FontSize);

        // フォントの色を取得
        Console.WriteLine("Font Color: " + list.FontColor);

        // フォーマットを取得
        Console.WriteLine("Font format: " + list.Format);

        //太字にチェック
        Console.WriteLine("Is bold: " + list.IsBold);

        // 斜体にチェック
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### 関連項目

* class [NumberList](../)
* 名前空間 [Aspose.Note](../../numberlist/)
* 組み立て [Aspose.Note](../../../)


