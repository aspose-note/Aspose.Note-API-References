---
title: Class MergeOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.MergeOptions クラス. ページのコレクションを結合するためのオプション
type: docs
weight: 340
url: /ja/net/aspose.note/mergeoptions/
---
## MergeOptions class

ページのコレクションを結合するためのオプション。

```csharp
public class MergeOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [MergeOptions](mergeoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | 提供されたページを単一ページとしてインポートするかどうかを示す値を取得または設定します。 |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | 挿入されたページを前のページの子として追加する必要があるかどうかを示す値を取得または設定します. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | インポートされたページが挿入される位置を取得または設定します。 |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | 単一ページとしてインポートされたときのページ間の間隔を取得または設定します。 |

### 例

5 ページごとにグループ化された PDF ドキュメントからすべてのページを 1 つの OneNote ページにインポートする方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

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

すべての PDF ドキュメントのページを 1 つの OneNote ページにマージしながら、一連の PDF ドキュメントからすべてのコンテンツをインポートする方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


