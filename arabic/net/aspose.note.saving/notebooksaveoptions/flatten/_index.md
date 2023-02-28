---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note لمرجع NET API
description: NotebookSaveOptions ملكية. الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان التسلسل الهرمي للأطفال في دفتر الملاحظات مسطحًا أم لا.
type: docs
weight: 20
url: /ar/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان التسلسل الهرمي للأطفال في دفتر الملاحظات مسطحًا أم لا.

```csharp
public bool Flatten { get; set; }
```

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

* class [NotebookSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../notebooksaveoptions/)
* المجسم [Aspose.Note](../../../)


