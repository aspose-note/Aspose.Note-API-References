---
title: PdfImporter.Import
second_title: Aspose.Note for .NET API 参考
description: PdfImporter 方法. 从提供的流中导入 PDF 文档的内容
type: docs
weight: 10
url: /zh/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

从提供的流中导入 PDF 文档的内容。

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 流. |
| options | PdfImportOptions | 选项。 |

### 返回值

的[`PdfImporter`](../).

### 也可以看看

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* 命名空间 [Aspose.Note.Importing](../../pdfimporter/)
* 部件 [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

从指定文件导入 PDF 文档的内容。

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| file | String | PDF 文件。 |
| options | PdfImportOptions | 选项。 |

### 返回值

的[`PdfImporter`](../).

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* 命名空间 [Aspose.Note.Importing](../../pdfimporter/)
* 部件 [Aspose.Note](../../../)


