---
title: "Document.DetectLayoutChanges"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Document. تكتشف جميع التغييرات التي تم إجراؤها على تخطيط المستند منذ استدعاء DetectLayoutChanges السابق. في حالة تعيين AutomaticLayoutChangesDetectionEnabled إلى true تُستخدم تلقائيًا في بداية تصدير المستند"
type: docs
weight: 90
url: /ar/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

تكتشف جميع التغييرات التي تم إجراؤها على تخطيط المستند منذ استدعاء `DetectLayoutChanges` السابق. في حالة تعيين [`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) إلى true، تُستخدم تلقائيًا في بداية تصدير المستند.

```csharp
public void DetectLayoutChanges()
```

## أمثلة

يوضح كيفية حفظ مستند بتنسيقات مختلفة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// تهيئة المستند الجديد
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// تهيئة الصفحة الجديدة
Page page = new Page();

// النمط الافتراضي لجميع النصوص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// إلحاق عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote بصيغ مختلفة، ضبط حجم خط النص واكتشاف تغييرات التخطيط يدويًا.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### انظر أيضًا

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


