---
title: "PdfSaveOptions.JpegQuality"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية PdfSaveOptions. يحصل أو يضبط قيمة تحدد جودة صور JPEG داخل مستند PDF. قد تتراوح القيمة من 0 إلى 100 حيث يعني 0 أسوأ جودة لكن أقصى ضغط و 100 يعني أفضل جودة لكن أقل ضغط"
type: docs
weight: 30
url: /ar/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

يحصل أو يضبط قيمة تحدد جودة صور JPEG داخل مستند PDF. يمكن أن تتراوح القيمة من 0 إلى 100 حيث 0 تعني أسوأ جودة ولكن أقصى ضغط و100 تعني أفضل جودة ولكن أقل ضغط.

```csharp
public int JpegQuality { get; set; }
```

## ملاحظات

القيمة الافتراضية هي 90.

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

* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


