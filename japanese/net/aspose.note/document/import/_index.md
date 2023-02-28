---
title: Document.Import
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. 提供された PDF ドキュメントから一連のページをインポートします
type: docs
weight: 110
url: /ja/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

提供された PDF ドキュメントから一連のページをインポートします。

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| stream | Stream | PDF ドキュメントを含むストリーム。 |
| importOptions | PdfImportOptions | PDF ドキュメントからページをインポートする方法のオプションを指定します。 |
| mergeOptions | MergeOptions | 提供されたページをマージする方法のオプションを指定します。 |

### 戻り値

ドキュメントへの参照を返します。

### 関連項目

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

提供された PDF ドキュメントから一連のページをインポートします。

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| file | String | PDF ドキュメントを含むファイル。 |
| importOptions | PdfImportOptions | PDF ドキュメントからページをインポートする方法のオプションを指定します。 |
| mergeOptions | MergeOptions | 提供されたページをマージする方法のオプションを指定します。 |

### 戻り値

ドキュメントへの参照を返します。

### 例

PDF ドキュメントのセットからすべてのページをページごとにインポートする方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


