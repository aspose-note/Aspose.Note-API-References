---
title: "MergeOptions.InsertAsChild"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية MergeOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب إضافة الصفحات المدخلة كأطفال للصفحة السابقة"
type: docs
weight: 30
url: /ar/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إضافة الصفحات المدخلة كأطفال للصفحة السابقة.

```csharp
public bool InsertAsChild { get; set; }
```

## أمثلة

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

### انظر أيضًا

* class [MergeOptions](../)
* namespace [Aspose.Note](../../mergeoptions/)
* assembly [Aspose.Note](../../../)


