---
title: "PdfSaveOptions.ImageCompression"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية PdfSaveOptions. تحصل أو تعين نوع الضغط المطبق على الصور في ملف PDF"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

يحصل أو يضبط نوع الضغط المطبق على الصور في ملف PDF.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

## أمثلة

يظهر كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدام ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### انظر أيضًا

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


