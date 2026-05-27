---
title: "PdfImporter.Import"
second_title: "Aspose.Note for .NET API 参考"
description: "PdfImporter 方法。从提供的流导入 PDF 文档的内容"
type: docs
weight: 10
url: /zh/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

从提供的流中导入 PDF 文档的内容。

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 选项 | PdfImportOptions | 这些选项。 |

### 返回值

此 [`PdfImporter`](../)。

### 另请参阅

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* namespace [Aspose.Note.Importing](../../pdfimporter/)
* assembly [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

从指定的文件中导入 PDF 文档的内容。

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件 | String | 此 PDF 文件。 |
| 选项 | PdfImportOptions | 这些选项。 |

### 返回值

此 [`PdfImporter`](../)。

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* namespace [Aspose.Note.Importing](../../pdfimporter/)
* assembly [Aspose.Note](../../../)


