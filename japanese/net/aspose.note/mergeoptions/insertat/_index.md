---
title: MergeOptions.InsertAt
second_title: Aspose.Note for .NET API リファレンス
description: MergeOptions 財産. インポートされたページが挿入される位置を取得または設定します
type: docs
weight: 40
url: /ja/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

インポートされたページが挿入される位置を取得または設定します。

```csharp
public int InsertAt { get; set; }
```

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException |  |

### 備考

値がターゲット ドキュメントのページ数より大きい場合、インポートされたページはドキュメントの末尾に追加されます。

### 例

すべての PDF ドキュメントのページをトップ レベルの OneNote ページの子として挿入しながら、一連の PDF ドキュメントからすべてのページをインポートする方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

### 関連項目

* class [MergeOptions](../)
* 名前空間 [Aspose.Note](../../mergeoptions/)
* 組み立て [Aspose.Note](../../../)


