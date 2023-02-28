---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note for .NET API 参考
description: PageSettings 财产. 获取无限高度的A4格式页面设置
type: docs
weight: 20
url: /zh/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

获取无限高度的A4格式页面设置。

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### 例子

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

* class [PageSettings](../)
* 命名空间 [Aspose.Note.Saving](../../pagesettings/)
* 部件 [Aspose.Note](../../../)


