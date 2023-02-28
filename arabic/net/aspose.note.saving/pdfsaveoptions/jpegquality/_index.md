---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note لمرجع NET API
description: PdfSaveOptions ملكية. الحصول على أو تعيين قيمة تحدد جودة صور JPEG داخل مستند PDF . قد تختلف القيمة من 0 إلى 100 حيث يعني 0 أسوأ جودة ولكن أقصى ضغط ويعني 100 أفضل جودة ولكن أقل ضغط .
type: docs
weight: 30
url: /ar/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

الحصول على أو تعيين قيمة تحدد جودة صور JPEG داخل مستند PDF . قد تختلف القيمة من 0 إلى 100 حيث يعني 0 أسوأ جودة ولكن أقصى ضغط ويعني 100 أفضل جودة ولكن أقل ضغط .

```csharp
public int JpegQuality { get; set; }
```

### ملاحظات

القيمة الافتراضية هي 90.

### أمثلة

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدم ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### أنظر أيضا

* class [PdfSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../pdfsaveoptions/)
* المجسم [Aspose.Note](../../../)


