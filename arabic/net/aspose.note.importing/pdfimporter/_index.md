---
title: Class PdfImporter
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Importing.PdfImporter فصل. الفئة التي توفر api لاستيراد المحتوى من المستندات بتنسيق PDF . تسمح واجهة برمجة التطبيقات بالاستيراد من مستند PDF الموجود إما في ملف أو في دفق باستخدام الخيارات المحددة. يتم تمرير خيارات الاستيراد باستخدامPdfImportOptions .
type: docs
weight: 270
url: /ar/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

الفئة التي توفر api لاستيراد المحتوى من المستندات بتنسيق PDF . تسمح واجهة برمجة التطبيقات بالاستيراد من مستند PDF الموجود إما في ملف أو في دفق باستخدام الخيارات المحددة. يتم تمرير خيارات الاستيراد باستخدام[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## طُرق

| اسم | وصف |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | يستورد محتوى مستند PDF من التدفق المقدم . |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | يستورد محتوى مستند PDF من ملف محدد. |

### أمثلة

يوضح كيفية استيراد كل الصفحات من مستند PDF الذي يجمع كل 5 صفحات إلى صفحة OneNote واحدة.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

### أنظر أيضا

* مساحة الاسم [Aspose.Note.Importing](../../aspose.note.importing/)
* المجسم [Aspose.Note](../../)


