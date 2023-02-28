---
title: MergeOptions.PageSpacing
second_title: Aspose.Note for .NET API リファレンス
description: MergeOptions 財産. 単一ページとしてインポートされたときのページ間の間隔を取得または設定します
type: docs
weight: 50
url: /ja/net/aspose.note/mergeoptions/pagespacing/
---
## MergeOptions.PageSpacing property

単一ページとしてインポートされたときのページ間の間隔を取得または設定します。

```csharp
public float PageSpacing { get; set; }
```

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

* class [MergeOptions](../)
* 名前空間 [Aspose.Note](../../mergeoptions/)
* 組み立て [Aspose.Note](../../../)


