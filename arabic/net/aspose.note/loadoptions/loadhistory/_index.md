---
title: "LoadOptions.LoadHistory"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "LoadOptions خاصية. يحصل على أو يضبط قيمة تشير إلى ما إذا كان محمل المستند يجب أن يتجاهل السجل. استخدم هذا الخيار لتقليل استهلاك الذاكرة ووحدة المعالجة المركزية. القيمة الافتراضية هي true"
type: docs
weight: 30
url: /ar/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب على محمل المستند تجاهل السجل. استخدم هذا الخيار لتقليل استهلاك الذاكرة والمعالج. القيمة الافتراضية هي `true`.

```csharp
public bool LoadHistory { get; set; }
```

## أمثلة

يظهر كيفية الحصول على تاريخ الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote.
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// احصل على الصفحة الأولى
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Note](../../loadoptions/)
* assembly [Aspose.Note](../../../)


