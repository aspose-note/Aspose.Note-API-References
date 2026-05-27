---
title: "PageSettings.A4NoHeightLimit"
second_title: "Aspose.Note for .NET API 参考"
description: "PageSettings 属性。获取 A4 格式页面的设置，且高度无限制"
type: docs
weight: 20
url: /zh/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

获取具有无限高度的 A4 格式页面的设置。

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

## 示例

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

* class [PageSettings](../)
* namespace [Aspose.Note.Saving](../../pagesettings/)
* assembly [Aspose.Note](../../../)


