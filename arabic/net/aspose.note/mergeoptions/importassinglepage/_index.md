---
title: MergeOptions.ImportAsSinglePage
second_title: Aspose.Note لمرجع NET API
description: MergeOptions ملكية. الحصول على أو تعيين قيمة تشير إلى ما إذا كان سيتم استيراد الصفحات المقدمة كصفحة واحدة.
type: docs
weight: 20
url: /ar/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

الحصول على أو تعيين قيمة تشير إلى ما إذا كان سيتم استيراد الصفحات المقدمة كصفحة واحدة.

```csharp
public bool ImportAsSinglePage { get; set; }
```

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

يوضح كيفية استيراد كل المحتوى من مجموعة مستندات PDF أثناء دمج الصفحات من كل مستند PDF إلى صفحة OneNote واحدة.

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

### أنظر أيضا

* class [MergeOptions](../)
* مساحة الاسم [Aspose.Note](../../mergeoptions/)
* المجسم [Aspose.Note](../../../)


