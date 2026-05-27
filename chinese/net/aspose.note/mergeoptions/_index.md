---
title: "类 MergeOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.MergeOptions 类。用于合并页面集合的选项"
type: docs
weight: 410
url: /zh/net/aspose.note/mergeoptions/
---
## MergeOptions class

用于合并页面集合的选项。

```csharp
public class MergeOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [MergeOptions](mergeoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | 获取或设置一个值，指示是否将提供的页面导入为单个页面。 |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | 获取或设置一个值，指示插入的页面是否应作为前一页面的子页面添加。 |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | 获取或设置导入页面将被插入的位置。 |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | 获取或设置在导入为单个页面时页面之间的间距。 |

## 示例

展示如何从 PDF 文档导入所有页面，将每 5 页分组为一个 OneNote 页面。

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


