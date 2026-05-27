---
title: "MergeOptions.InsertAt"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية MergeOptions. تحصل أو تعين الموضع الذي سيتم فيه إدراج الصفحات المستوردة"
type: docs
weight: 40
url: /ar/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

يحصل أو يعيّن الموضع الذي ستُدرج فيه الصفحات المستوردة.

```csharp
public int InsertAt { get; set; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentOutOfRangeException |  |

## ملاحظات

إذا كانت القيمة أكبر من عدد الصفحات في المستند الهدف، فستُضاف الصفحات المستوردة إلى نهاية المستند.

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


