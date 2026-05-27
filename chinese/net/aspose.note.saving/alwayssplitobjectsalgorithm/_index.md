---
title: "类 AlwaysSplitObjectsAlgorithm"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm 类。将对象拆分为多个部分，以防它不适合原始页面"
type: docs
weight: 630
url: /zh/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

在对象无法适应原始页面时，将其拆分为多个部分。

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | 默认构造函数。 |

## 示例

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


