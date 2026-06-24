---
title: "MergeOptions.ImportAsSinglePage"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية MergeOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب استيراد الصفحات المقدمة كصفحة واحدة"
type: docs
weight: 20
url: /ar/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب استيراد الصفحات المقدمة كصف واحد.

```csharp
public bool ImportAsSinglePage { get; set; }
```

## أمثلة

يعرض كيفية استيراد جميع الصفحات من مستند PDF مع تجميع كل 5 صفحات في صفحة OneNote واحدة.

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

يعرض كيفية استيراد جميع المحتويات من مجموعة مستندات PDF مع دمج صفحات كل مستند PDF في صفحة OneNote واحدة.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### انظر أيضًا

* class [MergeOptions](../)
* namespace [Aspose.Note](../../mergeoptions/)
* assembly [Aspose.Note](../../../)


