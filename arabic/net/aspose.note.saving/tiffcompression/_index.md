---
title: "التعداد TiffCompression"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "التعداد Aspose.Note.Saving.TiffCompression. يحدد نوع الضغط الذي يُستخدم عند حفظ مستند بتنسيق TIFF"
type: docs
weight: 960
url: /ar/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

يحدد نوع الضغط الذي يُستخدم عند حفظ مستند إلى تنسيق TIFF.

```csharp
public enum TiffCompression
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `1` | يحدد عدم وجود ضغط. |
| Rle | `2` | يحدد ضغط RLE. |
| Ccitt3 | `3` | يحدد ترميز الفاكس CCITT Group 3. |
| Ccitt4 | `4` | يحدد ترميز الفاكس CCITT Group 4. |
| Lzw | `5` | يحدد ضغط LZW. |
| PackBits | `32773` | يحدد ضغط Macintosh RLE. |
| Jpeg | `7` | يحدد ضغط JPEG DCT. |

## أمثلة

يظهر كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط PackBits.

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

يظهر كيفية حفظ المستند كصورة بتنسيق Tiff باستخدام ضغط CCITT Group 3 fax.

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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


