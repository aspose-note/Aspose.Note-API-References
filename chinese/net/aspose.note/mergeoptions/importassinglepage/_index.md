---
title: MergeOptions.ImportAsSinglePage
second_title: Aspose.Note for .NET API 参考
description: MergeOptions 财产. 获取或设置一个值该值指示是否将提供的页面作为单页导入
type: docs
weight: 20
url: /zh/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

获取或设置一个值，该值指示是否将提供的页面作为单页导入。

```csharp
public bool ImportAsSinglePage { get; set; }
```

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

* class [MergeOptions](../)
* 命名空间 [Aspose.Note](../../mergeoptions/)
* 部件 [Aspose.Note](../../../)


