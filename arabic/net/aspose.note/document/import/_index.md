---
title: Document.Import
second_title: Aspose.Note لمرجع NET API
description: Document طريقة. يستورد مجموعة من الصفحات من مستند PDF المقدم.
type: docs
weight: 110
url: /ar/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

يستورد مجموعة من الصفحات من مستند PDF المقدم.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | دفق مع مستند PDF . |
| importOptions | PdfImportOptions | يحدد الخيارات كيفية استيراد الصفحات من مستند PDF. |
| mergeOptions | MergeOptions | يحدد الخيارات الخاصة بكيفية دمج الصفحات المتوفرة. |

### قيمة الإرجاع

إرجاع المرجع إلى المستند.

### أنظر أيضا

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

يستورد مجموعة من الصفحات من مستند PDF المقدم.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| file | String | ملف به مستند PDF . |
| importOptions | PdfImportOptions | يحدد الخيارات كيفية استيراد الصفحات من مستند PDF. |
| mergeOptions | MergeOptions | يحدد الخيارات الخاصة بكيفية دمج الصفحات المتوفرة. |

### قيمة الإرجاع

إرجاع المرجع إلى المستند.

### أمثلة

يوضح كيفية استيراد كل الصفحات من مجموعة مستندات PDF صفحة بصفحة.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)


