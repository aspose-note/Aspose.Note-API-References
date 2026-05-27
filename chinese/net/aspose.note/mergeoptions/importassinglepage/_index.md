---
title: "MergeOptions.ImportAsSinglePage"
second_title: "Aspose.Note for .NET API 参考"
description: "MergeOptions 属性。获取或设置一个值，指示是否将提供的页面导入为单页"
type: docs
weight: 20
url: /zh/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

获取或设置一个值，指示是否将提供的页面导入为单个页面。

```csharp
public bool ImportAsSinglePage { get; set; }
```

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

* class [MergeOptions](../)
* namespace [Aspose.Note](../../mergeoptions/)
* assembly [Aspose.Note](../../../)


