---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note for .NET API リファレンス
description: MergeOptions 財産. 挿入されたページを前のページの子として追加する必要があるかどうかを示す値を取得または設定します.
type: docs
weight: 30
url: /ja/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

挿入されたページを前のページの子として追加する必要があるかどうかを示す値を取得または設定します.

```csharp
public bool InsertAsChild { get; set; }
```

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


