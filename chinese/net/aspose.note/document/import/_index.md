---
title: "Document.Import"
second_title: "Aspose.Note for .NET API 参考"
description: "Document 方法。导入提供的 PDF 文档中的一组页面"
type: docs
weight: 110
url: /zh/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import_1}

从提供的 PDF 文档导入一组页面。

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 包含 PDF 文档的流。 |
| importOptions | PdfImportOptions | 指定从 PDF 文档导入页面的选项。 |
| mergeOptions | MergeOptions | 指定合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

### 另请参阅

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_3}

从提供的 PDF 文档导入一组页面。

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | String | 包含 PDF 文档的文件。 |
| importOptions | PdfImportOptions | 指定从 PDF 文档导入页面的选项。 |
| mergeOptions | MergeOptions | 指定合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

## 示例

展示如何逐页从一组 PDF 文档中导入所有页面。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

展示如何将 PDF 文件导入到 OneNote 文档中。

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Pdf();

// 指定路径
var pdfFilePath = Path.Combine(dataDir, "sample.pdf");
var oneFilePath = Path.Combine(dataDir, "output.one");

// 将 PDF 导入 OneNote
var document = new Document();
document.Import(pdfFilePath);
document.Save(oneFilePath);
```

展示如何从一组 PDF 文档导入所有页面，同时将每个 PDF 文档的页面插入为顶层 OneNote 页面下的子页面。

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

展示如何从一组 PDF 文档导入所有内容，同时将每个 PDF 文档的页面合并为单个 OneNote 页面。

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

### 另请参阅

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(Stream, HtmlImportOptions, MergeOptions) {#import}

从提供的 HTML 文档导入一组页面。

```csharp
public Document Import(Stream stream, HtmlImportOptions importOptions, 
    MergeOptions mergeOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 包含 HTML 文档的流。 |
| importOptions | HtmlImportOptions | 指定从 HTML 文档导入页面的选项。 |
| mergeOptions | MergeOptions | 指定合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

### 另请参阅

* class [HtmlImportOptions](../../../aspose.note.importing/htmlimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(string, HtmlImportOptions, MergeOptions) {#import_2}

从提供的 HTML 文档导入一组页面。

```csharp
public Document Import(string file, HtmlImportOptions importOptions, 
    MergeOptions mergeOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | String | 包含 HTML 文档的文件。 |
| importOptions | HtmlImportOptions | 指定从 HTML 文档导入页面的选项。 |
| mergeOptions | MergeOptions | 指定合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

## 示例

展示如何将 HTML 文件导入到 OneNote 文档中。

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Html();

var htmlFilePath = Path.Combine(dataDir, "sample.html");
var oneFilePath = Path.Combine(dataDir, "output.one");

// 将 HTML 导入 OneNote
var doc = new Document();
doc.Import(htmlFilePath, new HtmlImportOptions());
doc.Save(oneFilePath);
```

展示如何将 Markdown 文件导入到 OneNote 文档中。

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Markdown();

var mdFilePath = Path.Combine(dataDir, "sample.md");
var htmlFilePath = Path.Combine(dataDir, "temp.html");
var oneFilePath = Path.Combine(dataDir, "output.one");

// 将 Markdown 转换为 HTML
Converter.ConvertMarkdown(mdFilePath, htmlFilePath);

// 将 HTML 导入 OneNote
var document = new Document();
document.Import(htmlFilePath, new HtmlImportOptions());
document.Save(oneFilePath);

Console.WriteLine("\nMarkdown document imported into OneNote successfully.");
```

### 另请参阅

* class [HtmlImportOptions](../../../aspose.note.importing/htmlimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


