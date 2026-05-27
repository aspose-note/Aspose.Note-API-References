---
title: "الفئة NotebookLoadOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.NotebookLoadOptions. الخيارات المستخدمة لتحميل دفتر ملاحظات"
type: docs
weight: 490
url: /ar/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

الخيارات المستخدمة لتحميل دفتر ملاحظات.

```csharp
public class NotebookLoadOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية صراحةً لاحقًا. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحميل المستندات الفرعية أثناء تحميل المستند الأصلي. |

## أمثلة

يوضح كيفية التعامل مع دفتر مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### انظر أيضًا

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


