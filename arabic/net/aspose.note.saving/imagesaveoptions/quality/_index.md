---
title: ImageSaveOptions.Quality
second_title: Aspose.Note لمرجع NET API
description: ImageSaveOptions ملكية. الحصول على أو تعيين قيمة تحدد جودة الصورة المحفوظة. يتم تمرير هذه القيمة إلى برنامج الترميز مثل System.Drawing.Imaging.Encoder.Quality parameter.
type: docs
weight: 40
url: /ar/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

الحصول على أو تعيين قيمة تحدد جودة الصورة المحفوظة. يتم تمرير هذه القيمة إلى برنامج الترميز مثل System.Drawing.Imaging.Encoder.Quality parameter.

```csharp
public int Quality { get; set; }
```

### ملاحظات

يتراوح نطاق القيم المفيدة لفئة الجودة من 0 إلى 100. كلما انخفض الرقم المحدد ، زاد الضغط وبالتالي انخفضت جودة الصورة . يمنحك الصفر أدنى جودة للصورة و 100 أعلى . القيمة الافتراضية هي 90.

### أمثلة

يوضح كيفية ضبط جودة الصورة عند حفظ المستند كصورة بتنسيق JPEG.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

يوضح كيفية حفظ مستند كصورة بتنسيق Tiff باستخدام ضغط Jpeg.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### أنظر أيضا

* class [ImageSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../imagesaveoptions/)
* المجسم [Aspose.Note](../../../)


