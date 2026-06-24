---
title: "ImageSaveOptions.TiffCompression"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية ImageSaveOptions. تحصل أو تعيين نوع الضغط المستخدم عند حفظ الصور المولدة بتنسيق TIFF"
type: docs
weight: 60
url: /ar/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

يحصل أو يعيّن نوع الضغط المستخدم عند حفظ الصور المُولَّدة بتنسيق TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## أمثلة

يوضح كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط PackBits.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

يوضح كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط Jpeg.

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

يوضح كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط الفاكس CCITT Group 3.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// احفظ المستند.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### انظر أيضًا

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Note.Saving](../../imagesaveoptions/)
* assembly [Aspose.Note](../../../)


