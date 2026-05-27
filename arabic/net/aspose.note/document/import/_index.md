---
title: "Document.Import"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Document. تستورد مجموعة من الصفحات من مستند PDF المقدم"
type: docs
weight: 110
url: /ar/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import_1}

يستورد مجموعة من الصفحات من مستند PDF المقدم.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | تدفق يحتوي على مستند PDF. |
| importOptions | PdfImportOptions | يحدد الخيارات التي يتم من خلالها استيراد الصفحات من مستند PDF. |
| mergeOptions | MergeOptions | يحدد الخيارات التي يتم من خلالها دمج الصفحات المقدمة. |

### قيمة الإرجاع

يعيد المرجع إلى المستند.

### انظر أيضًا

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_3}

يستورد مجموعة من الصفحات من مستند PDF المقدم.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | String | ملف يحتوي على مستند PDF. |
| importOptions | PdfImportOptions | يحدد الخيارات التي يتم من خلالها استيراد الصفحات من مستند PDF. |
| mergeOptions | MergeOptions | يحدد الخيارات التي يتم من خلالها دمج الصفحات المقدمة. |

### قيمة الإرجاع

يعيد المرجع إلى المستند.

## أمثلة

يوضح كيفية استيراد جميع الصفحات من مجموعة من مستندات PDF صفحةً بصفحة.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

يوضح كيفية استيراد ملف PDF إلى مستند OneNote.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Pdf();

// حدد المسارات
var pdfFilePath = Path.Combine(dataDir, "sample.pdf");
var oneFilePath = Path.Combine(dataDir, "output.one");

// استيراد PDF إلى OneNote
var document = new Document();
document.Import(pdfFilePath);
document.Save(oneFilePath);
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

يعرض كيفية استيراد جميع المحتويات من مجموعة مستندات PDF مع دمج صفحات كل مستند PDF إلى صفحة OneNote واحدة.

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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(Stream, HtmlImportOptions, MergeOptions) {#import}

يستورد مجموعة من الصفحات من مستند HTML المقدم.

```csharp
public Document Import(Stream stream, HtmlImportOptions importOptions, 
    MergeOptions mergeOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | Stream | تدفق يحتوي على مستند HTML. |
| importOptions | HtmlImportOptions | يحدد الخيارات التي يتم من خلالها استيراد الصفحات من مستند HTML. |
| mergeOptions | MergeOptions | يحدد الخيارات التي يتم من خلالها دمج الصفحات المقدمة. |

### قيمة الإرجاع

يعيد المرجع إلى المستند.

### انظر أيضًا

* class [HtmlImportOptions](../../../aspose.note.importing/htmlimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(string, HtmlImportOptions, MergeOptions) {#import_2}

يستورد مجموعة من الصفحات من مستند HTML المقدم.

```csharp
public Document Import(string file, HtmlImportOptions importOptions, 
    MergeOptions mergeOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ملف | String | ملف يحتوي على مستند HTML. |
| importOptions | HtmlImportOptions | يحدد الخيارات التي يتم من خلالها استيراد الصفحات من مستند HTML. |
| mergeOptions | MergeOptions | يحدد الخيارات التي يتم من خلالها دمج الصفحات المقدمة. |

### قيمة الإرجاع

يعيد المرجع إلى المستند.

## أمثلة

يوضح كيفية استيراد ملف HTML إلى مستند OneNote.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Html();

var htmlFilePath = Path.Combine(dataDir, "sample.html");
var oneFilePath = Path.Combine(dataDir, "output.one");

// استيراد HTML إلى OneNote
var doc = new Document();
doc.Import(htmlFilePath, new HtmlImportOptions());
doc.Save(oneFilePath);
```

يظهر كيفية استيراد ملف Markdown إلى مستند OneNote.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Markdown();

var mdFilePath = Path.Combine(dataDir, "sample.md");
var htmlFilePath = Path.Combine(dataDir, "temp.html");
var oneFilePath = Path.Combine(dataDir, "output.one");

// تحويل Markdown إلى HTML
Converter.ConvertMarkdown(mdFilePath, htmlFilePath);

// استيراد HTML إلى OneNote
var document = new Document();
document.Import(htmlFilePath, new HtmlImportOptions());
document.Save(oneFilePath);

Console.WriteLine("\nMarkdown document imported into OneNote successfully.");
```

### انظر أيضًا

* class [HtmlImportOptions](../../../aspose.note.importing/htmlimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


