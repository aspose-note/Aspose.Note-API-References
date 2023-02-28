---
title: Page.Author
second_title: Aspose.Note لمرجع NET API
description: Page ملكية. الحصول على أو تعيين المؤلف.
type: docs
weight: 20
url: /ar/net/aspose.note/page/author/
---
## Page.Author property

الحصول على أو تعيين المؤلف.

```csharp
public string Author { get; set; }
```

### أمثلة

يوضح كيفية الحصول على معلومات التعريف حول الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

يوضح كيفية الحصول على محفوظات الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote
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

### أنظر أيضا

* class [Page](../)
* مساحة الاسم [Aspose.Note](../../page/)
* المجسم [Aspose.Note](../../../)


