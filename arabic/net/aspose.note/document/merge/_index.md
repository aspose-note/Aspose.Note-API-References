---
title: "Document.Merge"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Document. دمج مجموعة من الصفحات إلى المستند"
type: docs
weight: 120
url: /ar/net/aspose.note/document/merge/
---
## Document.Merge method

يدمج مجموعة من الصفحات إلى المستند.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صفحات | IEnumerable`1 | مجموعة من الصفحات. |
| mergeOptions | MergeOptions | يحدد الخيارات التي يتم من خلالها دمج الصفحات المقدمة. |

### قيمة الإرجاع

يعيد المرجع إلى المستند.

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

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


