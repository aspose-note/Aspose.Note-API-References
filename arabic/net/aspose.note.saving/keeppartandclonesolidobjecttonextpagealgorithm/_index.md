---
title: "الفئة KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm. يضيف الجزء العلوي من الكائنات إلى أسفل الصفحة ويستنسخ الكائن بالكامل إلى الصفحة التالية في حال لم يتناسب مع الصفحة الأصلية."
type: docs
weight: 810
url: /ar/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

يضيف الجزء العلوي من الكائن إلى أسفل الصفحة ويستنسخ الكائن بالكامل إلى الصفحة التالية في حال لم يتناسب مع الصفحة الأصلية.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | ينشئ مثيلاً جديداً من الفئة `KeepPartAndCloneSolidObjectToNextPageAlgorithm`، باستخدام حد الارتفاع الافتراضي للجزء المستنسخ. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | ينشئ مثيلاً جديداً من الفئة `KeepPartAndCloneSolidObjectToNextPageAlgorithm`، باستخدام حد ارتفاع محدد للجزء المستنسخ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | يحصل على حد الارتفاع للجزء المستنسخ. |

## الحقول

| الاسم | الوصف |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | الحجم الأقصى الافتراضي للجزء المستنسخ. |

## أمثلة

عند حفظ صفحات OneNote الطويلة بتنسيق pdf يتم تقسيمها عبر صفحات. يوضح المثال كيفية تكوين منطق التقسيم للكائنات الموجودة على فواصل الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

عند حفظ صفحات OneNote الطويلة بتنسيق PDF يتم تقسيمها عبر صفحات متعددة. يوضح المثال كيفية تكوين منطق التقسيم للكائنات الموجودة على فواصل الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
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

### انظر أيضًا

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


