---
title: "类 PdfImporter"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Importing.PdfImporter 类。提供用于从 PDF 格式文档导入内容的 API。该 API 允许使用指定的选项从文件或流中的 PDF 文档导入。导入选项通过 PdfImportOptions 传递"
type: docs
weight: 290
url: /zh/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

提供用于从 PDF 格式文档导入内容的 API 的类。该 API 允许使用指定的选项从文件或流中的 PDF 文档导入。导入选项通过 [`PdfImportOptions`](../pdfimportoptions/) 传递。

```csharp
public static class PdfImporter
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | 从提供的流中导入 PDF 文档的内容。 |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | 从指定的文件中导入 PDF 文档的内容。 |

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

### 另请参阅

* namespace [Aspose.Note.Importing](../../aspose.note.importing/)
* assembly [Aspose.Note](../../)


