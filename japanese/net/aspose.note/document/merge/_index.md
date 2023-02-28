---
title: Document.Merge
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. 一連のページをドキュメントに結合します
type: docs
weight: 120
url: /ja/net/aspose.note/document/merge/
---
## Document.Merge method

一連のページをドキュメントに結合します。

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pages | IEnumerable`1 | ページのセット. |
| mergeOptions | MergeOptions | 提供されたページをマージする方法のオプションを指定します。 |

### 戻り値

ドキュメントへの参照を返します。

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

### 関連項目

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


