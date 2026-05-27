---
title: "ImageSaveOptions.Resolution"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية ImageSaveOptions. يحصل أو يضبط الدقة للصور المُولَّدة بوحدة النقاط في البوصة"
type: docs
weight: 50
url: /ar/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

يحصل أو يضبط الدقة للصور المُولَّدة، بوحدة النقاط في البوصة.

```csharp
public float Resolution { get; set; }
```

## ملاحظات

القيمة الافتراضية هي 96.

## أمثلة

يعرض كيفية ضبط دقة الصورة عند حفظ المستند كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

يوضح كيفية حفظ الدفتر كصورة مع الخيارات المحددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// احفظ الدفتر
notebook.Save(dataDir, notebookSaveOptions);
```

يوضح كيفية حفظ الدفتر المسطح كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// احفظ الدفتر
notebook.Save(dataDir, notebookSaveOptions);
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Note.Saving](../../imagesaveoptions/)
* assembly [Aspose.Note](../../../)


