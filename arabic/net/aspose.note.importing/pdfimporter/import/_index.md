---
title: PdfImporter.Import
second_title: Aspose.Note لمرجع NET API
description: PdfImporter طريقة. يستورد محتوى مستند PDF من التدفق المقدم .
type: docs
weight: 10
url: /ar/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

يستورد محتوى مستند PDF من التدفق المقدم .

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | الدفق . |
| options | PdfImportOptions | الخيارات . |

### قيمة الإرجاع

ملف[`PdfImporter`](../) .

### أنظر أيضا

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* مساحة الاسم [Aspose.Note.Importing](../../pdfimporter/)
* المجسم [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

يستورد محتوى مستند PDF من ملف محدد.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| file | String | ملف PDF . |
| options | PdfImportOptions | الخيارات . |

### قيمة الإرجاع

ملف[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* مساحة الاسم [Aspose.Note.Importing](../../pdfimporter/)
* المجسم [Aspose.Note](../../../)


