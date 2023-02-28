---
title: Class NotebookSaveOptions
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.NotebookSaveOptions فصل. فئة أساسية مجردة تمثل خيارات حفظ الكمبيوتر المحمول لتنسيق معين.
type: docs
weight: 790
url: /ar/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

فئة أساسية مجردة تمثل خيارات حفظ الكمبيوتر المحمول لتنسيق معين.

```csharp
public abstract class NotebookSaveOptions
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان يجب حفظ المستندات الفرعية بشكل صريح . |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان التسلسل الهرمي للأطفال في دفتر الملاحظات مسطحًا أم لا. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | يحصل على التنسيق الذي تم حفظ دفتر الملاحظات به. |

## طُرق

| اسم | وصف |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | يحصل على خيارات الحفظ لجميع المستندات التابعة للدفتر. |

### أمثلة

يوضح كيفية حفظ دفتر ملاحظات مسطح بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// حفظ دفتر الملاحظات
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

يوضح كيفية حفظ دفتر الملاحظات المسطح كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
```

### أنظر أيضا

* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


