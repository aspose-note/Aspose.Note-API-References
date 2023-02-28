---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm فصل. يقسم الكائن إلى عدة أجزاء في حالة عدم احتوائه في الصفحة الأصلية.
type: docs
weight: 550
url: /ar/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

يقسم الكائن إلى عدة أجزاء في حالة عدم احتوائه في الصفحة الأصلية.

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | Default_Constructor |

### أمثلة

عندما يتم حفظ صفحات OneNote الطويلة بتنسيق pdf ، يتم تقسيمها عبر الصفحات. يوضح المثال كيفية تكوين منطق تقسيم الكائنات الموجودة في فواصل الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### أنظر أيضا

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


