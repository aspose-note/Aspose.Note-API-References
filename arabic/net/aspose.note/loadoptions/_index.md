---
title: "الفئة LoadOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.LoadOptions. الخيارات المستخدمة لتحميل مستند."
type: docs
weight: 380
url: /ar/net/aspose.note/loadoptions/
---
## LoadOptions class

الخيارات المستخدمة لتحميل مستند.

```csharp
public class LoadOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [LoadOptions](loadoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | يحصل أو يضبط كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حال عدم حماية المستند بكلمة مرور. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب على محمل المستند تجاهل السجل. استخدم هذا الخيار لتقليل استهلاك الذاكرة والمعالج. القيمة الافتراضية هي `true`. |

## أمثلة

يعرض كيفية التعامل مع مستند مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

يوضح كيفية التعامل مع دفتر مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


