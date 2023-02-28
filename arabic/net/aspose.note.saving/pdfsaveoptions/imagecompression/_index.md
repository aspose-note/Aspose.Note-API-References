---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note لمرجع NET API
description: PdfSaveOptions ملكية. الحصول على أو تحديد نوع الضغط المطبق على الصور في ملف PDF.
type: docs
weight: 20
url: /ar/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

الحصول على أو تحديد نوع الضغط المطبق على الصور في ملف PDF.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../pdfsaveoptions/)
* المجسم [Aspose.Note](../../../)


