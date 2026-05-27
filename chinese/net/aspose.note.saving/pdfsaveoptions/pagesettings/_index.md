---
title: "PdfSaveOptions.PageSettings"
second_title: "Aspose.Note for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置文档中每页的页面设置。默认情况下取决于 CurrentUICulture，US 文化使用 Letter 设置，其他使用 A4 设置"
type: docs
weight: 40
url: /zh/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

获取或设置文档中每页的页面设置。默认情况下取决于 CurrentUICulture，*美国地区使用信纸尺寸，其他地区使用 A4 尺寸。

```csharp
public PageSettings PageSettings { get; set; }
```

## 示例

展示如何将文档保存为 Pdf 格式并使用 Letter 页面布局。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

展示如何将文档保存为 Pdf 格式并使用 A4 页面布局且不限制高度。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### 另请参阅

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


