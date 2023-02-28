---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm 班级. 将对象拆分为多个部分以防原始页面放不下
type: docs
weight: 550
url: /zh/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

将对象拆分为多个部分，以防原始页面放不下。

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | 默认构造函数。 |

### 例子

当 OneNote 长页面以 pdf 格式保存时，它们会被拆分成多个页面。该示例显示如何配置位于分页符处的对象的拆分逻辑。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// 或者
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### 也可以看看

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* 命名空间 [Aspose.Note.Saving](../../aspose.note.saving/)
* 部件 [Aspose.Note](../../)


