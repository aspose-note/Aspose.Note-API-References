---
title: "类 KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm 类。将对象的顶部部分添加到页面底部，并在对象不适合原页面时将完整对象克隆到下一页"
type: docs
weight: 810
url: /zh/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

将对象的顶部添加到页面底部，并在对象无法适应原始页面时将完整对象克隆到下一页。

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | 初始化 `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 类的新实例，使用克隆部分的默认高度限制。 |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | 初始化 `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 类的新实例，使用克隆部分的特定高度限制。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | 获取克隆部件的高度限制。 |

## 字段

| 名称 | 描述 |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | 克隆部件的默认最大尺寸。 |

## 示例

当长的 OneNote 页面以 PDF 格式保存时，它们会被拆分到多个页面。示例展示如何配置位于页面换页处对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

当长的 OneNote 页面以 PDF 格式保存时，它们会被拆分到多个页面。示例展示如何配置位于页面换行处对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 或
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### 另请参阅

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


