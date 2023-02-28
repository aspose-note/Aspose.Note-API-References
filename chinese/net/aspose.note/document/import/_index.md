---
title: Document.Import
second_title: Aspose.Note for .NET API 参考
description: Document 方法. 从提供的 PDF 文档中导入一组页面
type: docs
weight: 110
url: /zh/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

从提供的 PDF 文档中导入一组页面。

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 带有 PDF 文档的流。 |
| importOptions | PdfImportOptions | 指定如何从 PDF 文档导入页面的选项。 |
| mergeOptions | MergeOptions | 指定如何合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

### 也可以看看

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

从提供的 PDF 文档中导入一组页面。

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| file | String | 带有 PDF 文档的文件。 |
| importOptions | PdfImportOptions | 指定如何从 PDF 文档导入页面的选项。 |
| mergeOptions | MergeOptions | 指定如何合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

### 例子

显示如何逐页导入一组 PDF 文档中的所有页面。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

显示如何从一组 PDF 文档导入所有页面，同时从每个 PDF 文档插入页面作为顶级 OneNote 页面的子页面。

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

展示如何从一组 PDF 文档导入所有内容，同时将每个 PDF 文档的页面合并到单个 OneNote 页面。

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

### 也可以看看

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


