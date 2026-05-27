---
title: "PdfImporter.Import"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة PdfImporter. تستورد محتوى مستند PDF من تدفق مُقدم"
type: docs
weight: 10
url: /ar/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

يستورد محتوى مستند PDF من تدفق مُقدم.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | التدفق. |
| خيارات | PdfImportOptions | الخيارات. |

### قيمة الإرجاع

ال [`PdfImporter`](../).

### انظر أيضًا

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* namespace [Aspose.Note.Importing](../../pdfimporter/)
* assembly [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

يستورد محتوى مستند PDF من ملف محدد.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | String | ملف PDF. |
| خيارات | PdfImportOptions | الخيارات. |

### قيمة الإرجاع

ال [`PdfImporter`](../).

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* namespace [Aspose.Note.Importing](../../pdfimporter/)
* assembly [Aspose.Note](../../../)


