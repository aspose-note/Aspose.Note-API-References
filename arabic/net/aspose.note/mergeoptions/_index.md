---
title: Class MergeOptions
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.MergeOptions فصل. خيارات دمج مجموعة من الصفحات .
type: docs
weight: 340
url: /ar/net/aspose.note/mergeoptions/
---
## MergeOptions class

خيارات دمج مجموعة من الصفحات .

```csharp
public class MergeOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان سيتم استيراد الصفحات المقدمة كصفحة واحدة. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب إضافة الصفحات المدرجة كأبناء الصفحة السابقة. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | الحصول على أو تحديد الموضع الذي سيتم فيه إدراج الصفحات المستوردة. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | الحصول على التباعد بين الصفحات أو تعيينه عند استيرادها كصفحة واحدة. |

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

يوضح كيفية استيراد كل الصفحات من مجموعة مستندات PDF أثناء إدراج الصفحات من كل مستند PDF كأطفال لصفحة OneNote ذات المستوى الأعلى.

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

* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


