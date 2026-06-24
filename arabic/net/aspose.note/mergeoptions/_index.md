---
title: "الفئة MergeOptions"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "الفئة Aspose.Note.MergeOptions. الخيارات لدمج مجموعة من الصفحات"
type: docs
weight: 410
url: /ar/net/aspose.note/mergeoptions/
---
## MergeOptions class

الخيارات لدمج مجموعة من الصفحات.

```csharp
public class MergeOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [MergeOptions](mergeoptions/)() | الباني الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب استيراد الصفحات المقدمة كصف واحد. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إضافة الصفحات المُدخلة كأطفال للصفحة السابقة. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | يحصل أو يعيّن الموضع الذي ستُدرج فيه الصفحات المستوردة. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | يحصل أو يعيّن التباعد بين الصفحات عند استيرادها كصف واحد. |

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

يعرض كيفية استيراد جميع الصفحات من مجموعة مستندات PDF مع إدراج صفحات كل مستند PDF كأطفال لصفحة OneNote المستوى الأعلى.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


