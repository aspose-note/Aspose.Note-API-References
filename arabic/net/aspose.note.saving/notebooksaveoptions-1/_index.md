---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions فصل. فئة أساسية مجردة تمثل خيارات حفظ الكمبيوتر المحمول لتنسيق معين وتوفر خيارات حفظ عامة لجميع العقد التابعة للمستند .
type: docs
weight: 800
url: /ar/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

فئة أساسية مجردة تمثل خيارات حفظ الكمبيوتر المحمول لتنسيق معين وتوفر خيارات حفظ عامة لجميع العقد التابعة للمستند .

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| معامل | وصف |
| --- | --- |
| TDocumentSaveOptions | خيارات الحفظ لكافة المستندات التابعة لدفتر الملاحظات . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب حفظ المستندات الفرعية بشكل صريح . |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | الحصول على أو تعيين خيارات الحفظ لجميع المستندات التابعة لدفتر الملاحظات. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان التسلسل الهرمي للأطفال في دفتر الملاحظات مسطحًا أم لا. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | يحصل على التنسيق الذي تم حفظ دفتر الملاحظات به. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | يحصل على خيارات الحفظ لجميع المستندات التابعة للدفتر. |

### أمثلة

يوضح كيفية حفظ دفتر الملاحظات بتنسيق pdf بخيارات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
```

### أنظر أيضا

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


