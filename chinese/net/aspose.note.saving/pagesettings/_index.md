---
title: Class PageSettings
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Saving.PageSettings 班级. 表示页面的布局设置
type: docs
weight: 820
url: /zh/net/aspose.note.saving/pagesettings/
---
## PageSettings class

表示页面的布局设置。

```csharp
public class PageSettings
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | 获取 A4 格式页面的设置。 |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | 获取无限高度的A4格式页面设置。 |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | 获取信件格式页面的设置。 |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | 获取无限高度的 Letter-format 页面设置。 |

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

* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving/)
* 部件 [Aspose.Note](../../)


