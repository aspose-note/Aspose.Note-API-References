---
title: Class PdfImporter
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Importing.PdfImporter 班级. 提供 api 的类以从 PDF 格式的文档导入内容 api 允许使用指定的选项从位于文件或流中的 PDF 文档导入 导入选项使用PdfImportOptions.
type: docs
weight: 270
url: /zh/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

提供 api 的类以从 PDF 格式的文档导入内容。 api 允许使用指定的选项从位于文件或流中的 PDF 文档导入。 导入选项使用[`PdfImportOptions`](../pdfimportoptions/).

```csharp
public static class PdfImporter
```

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | 从提供的流中导入 PDF 文档的内容。 |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | 从指定文件导入 PDF 文档的内容。 |

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

* 命名空间 [Aspose.Note.Importing](../../aspose.note.importing/)
* 部件 [Aspose.Note](../../)


