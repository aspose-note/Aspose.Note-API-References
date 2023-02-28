---
title: Class PdfImporter
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Importing.PdfImporter クラス. PDF 形式のドキュメントからコンテンツをインポートするための API を提供するクラスPdfImportOptions.
type: docs
weight: 270
url: /ja/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

PDF 形式のドキュメントからコンテンツをインポートするための API を提供するクラス。[`PdfImportOptions`](../pdfimportoptions/).

```csharp
public static class PdfImporter
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | 提供されたストリームから PDF ドキュメントのコンテンツをインポートします。 |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | 指定したファイルから PDF ドキュメントのコンテンツをインポートします。 |

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

* 名前空間 [Aspose.Note.Importing](../../aspose.note.importing/)
* 組み立て [Aspose.Note](../../)


