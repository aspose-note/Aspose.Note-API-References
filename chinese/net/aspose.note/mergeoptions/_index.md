---
title: Class MergeOptions
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.MergeOptions 班级. 合并页面集合的选项
type: docs
weight: 340
url: /zh/net/aspose.note/mergeoptions/
---
## MergeOptions class

合并页面集合的选项。

```csharp
public class MergeOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [MergeOptions](mergeoptions/)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | 获取或设置一个值，该值指示是否将提供的页面作为单页导入。 |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | 获取或设置一个值，该值指示插入的页面是否应添加为上一页的子页面。 |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | 获取或设置将插入导入页面的位置。 |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | 获取或设置作为单个页面导入时页面之间的间距。 |

### 例子

演示如何将每 5 页分组的 PDF 文档中的所有页面导入到单个 OneNote 页面。

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

* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


