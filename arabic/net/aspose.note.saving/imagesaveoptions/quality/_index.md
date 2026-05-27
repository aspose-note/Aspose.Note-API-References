---
title: "ImageSaveOptions.Quality"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية ImageSaveOptions. يحصل أو يضبط قيمة تحدد جودة الصورة المحفوظة. تُمرّر هذه القيمة إلى برنامج الترميز كمعامل System.Drawing.Imaging.Encoder.Quality"
type: docs
weight: 40
url: /ar/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

يحصل أو يضبط قيمة تحدد جودة الصورة المحفوظة. تُمرّر هذه القيمة إلى الترميز كمعامل System.Drawing.Imaging.Encoder.Quality.

```csharp
public int Quality { get; set; }
```

## ملاحظات

نطاق القيم المفيدة لفئة الجودة هو من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. الصفر يعطيك أدنى جودة للصورة و100 أعلى جودة. القيمة الافتراضية هي 90.

## أمثلة

يعرض كيفية ضبط جودة الصورة عند حفظ المستند كصورة بتنسيق JPEG.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

يظهر كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط Jpeg.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Note.Saving](../../imagesaveoptions/)
* assembly [Aspose.Note](../../../)


