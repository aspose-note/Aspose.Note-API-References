---
title: "الفئة PdfImporter"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Importing.PdfImporter. الفئة التي توفر واجهة برمجة تطبيقات لاستيراد المحتوى من المستندات بصيغة PDF. تسمح الواجهة باستيراد مستند PDF موجود إما في ملف أو في تدفق باستخدام الخيارات المحددة. يتم تمرير خيارات الاستيراد باستخدام PdfImportOptions"
type: docs
weight: 290
url: /ar/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

الفئة التي توفر واجهة برمجة تطبيقات لاستيراد المحتوى من المستندات بصيغة PDF. تسمح الواجهة باستيراد مستند PDF موجود إما في ملف أو في تدفق باستخدام الخيارات المحددة. يتم تمرير خيارات الاستيراد باستخدام [`PdfImportOptions`](../pdfimportoptions/).

```csharp
public static class PdfImporter
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | يستورد محتوى مستند PDF من تدفق مُقدم. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | يستورد محتوى مستند PDF من ملف محدد. |

## أمثلة

يعرض كيفية استيراد جميع الصفحات من مستند PDF مع تجميع كل 5 صفحات إلى صفحة OneNote واحدة.

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

### انظر أيضًا

* namespace [Aspose.Note.Importing](../../aspose.note.importing/)
* assembly [Aspose.Note](../../)


