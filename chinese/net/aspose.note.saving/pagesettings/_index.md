---
title: "类 PageSettings"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.PageSettings 类。表示页面的布局设置"
type: docs
weight: 900
url: /zh/net/aspose.note.saving/pagesettings/
---
## PageSettings class

表示页面的布局设置。

```csharp
public class PageSettings
```

## 属性

| 名称 | 描述 |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | 获取 A4 格式页面的设置。 |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | 获取具有无限高度的 A4 格式页面的设置。 |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | 获取 Letter 格式页面的设置。 |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | 获取具有无限高度的 Letter 格式页面的设置。 |

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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


