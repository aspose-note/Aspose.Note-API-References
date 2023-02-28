---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note for .NET API 参考
description: PdfSaveOptions 财产. 获取或设置文档中每一页的页面设置 默认取决于 CurrentUICulture美国文化有字母设置其他文化有 A4 设置
type: docs
weight: 40
url: /zh/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

获取或设置文档中每一页的页面设置。 默认取决于 CurrentUICulture，*美国文化有字母设置，其他文化有 A4 设置。

```csharp
public PageSettings PageSettings { get; set; }
```

### 例子

展示如何使用 Letter 页面布局将文档保存为 Pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

演示如何将文档保存为 A4 页面布局且没有高度限制的 Pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### 也可以看看

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../pdfsaveoptions/)
* 部件 [Aspose.Note](../../../)


