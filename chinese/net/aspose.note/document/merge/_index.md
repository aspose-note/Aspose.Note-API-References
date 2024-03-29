---
title: Document.Merge
second_title: Aspose.Note for .NET API 参考
description: Document 方法. 将一组页面合并到文档中
type: docs
weight: 120
url: /zh/net/aspose.note/document/merge/
---
## Document.Merge method

将一组页面合并到文档中。

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pages | IEnumerable`1 | 一组页面。 |
| mergeOptions | MergeOptions | 指定如何合并提供的页面的选项。 |

### 返回值

返回对文档的引用。

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

### 也可以看看

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


