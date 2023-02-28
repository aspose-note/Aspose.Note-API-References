---
title: PdfImporter.Import
second_title: Aspose.Note for .NET API リファレンス
description: PdfImporter 方法. 提供されたストリームから PDF ドキュメントのコンテンツをインポートします
type: docs
weight: 10
url: /ja/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

提供されたストリームから PDF ドキュメントのコンテンツをインポートします。

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | ストリーム. |
| options | PdfImportOptions | オプション. |

### 戻り値

[`PdfImporter`](../).

### 関連項目

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* 名前空間 [Aspose.Note.Importing](../../pdfimporter/)
* 組み立て [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

指定したファイルから PDF ドキュメントのコンテンツをインポートします。

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| file | String | PDF ファイル。 |
| options | PdfImportOptions | オプション. |

### 戻り値

[`PdfImporter`](../).

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* 名前空間 [Aspose.Note.Importing](../../pdfimporter/)
* 組み立て [Aspose.Note](../../../)


